# 🚀 Nuxt.js SSR on AWS Serverless Stack (Lambda + API Gateway + S3)

Nuxt.js Serverless Server-side Rendering Starter on AWS Serverless Stack (Lambda + API Gateway + S3) with *Serverless Framework*

### Pre-Installed
- Nuxt.js 2.8.1
- Serverless Framework
- TypeScript
- Sass (SCSS)
- TSLint


## Configuration
Edit `serverless.yml`

```yaml
service: nuxt-serverless  # 1. Edit whole service name

plugins:
  - serverless-s3-sync
  - serverless-apigw-binary
  - serverless-dotenv-plugin

package:
  individually: true
  excludeDevDependencies: true

provider:
  name: aws
  runtime: nodejs10.x
  stage: ${opt:stage, 'dev'}
  region: us-east-1  # 2. Edit AWS region name

custom:
  #######################################
  # Unique ID included in resource names.
  # Replace it with a random value for every first distribution.
  # https://www.random.org/strings/?num=1&len=6&digits=on&loweralpha=on&unique=on&format=html&rnd=new
  stackId: abcdef  # 3. Update Random Stack ID
  #######################################

  buckets:
    ASSETS_BUCKET_NAME: ${self:service}-${self:custom.stackId}-${self:provider.stage}-assets
    STATIC_BUCKET_NAME: ${self:service}-${self:custom.stackId}-${self:provider.stage}-static
  s3Sync:
    - bucketName: ${self:custom.buckets.ASSETS_BUCKET_NAME}
      localDir: .nuxt/dist/client
    - bucketName: ${self:custom.buckets.STATIC_BUCKET_NAME}
      localDir: static
  apigwBinary:
    types:
      - '*/*'
```

## Build Setup
```bash
# Install dependencies
$ npm install

# Serve develop server at localhost:3000 using Nuxt.js
$ npm run dev

# Build
$ npm run build

# Prod server start with built assets
$ npm run start

## SERVERLESS DEPLOYMENT ##
# Build and deploy the function and bundled assets
$ npm run deploy:dev
$ npm run deploy:stage
$ npm run deploy:prod

# Remove Deployment
$ npm run undeploy:dev
$ npm run undeploy:stage
$ npm run undeploy:prod
```

## Environment Variables
- update `.env.development`, `.env.production`.
- If env variable key started with `NUXT_APP`, it injected to client in `this.$store.state.environments`.
- WARNING!: Untrack the `.env.development` and the `.env.production` before commit

## Folder Structure
- `/api`: You can create a sub-API based on Express.js. dynamic ajax Set-Cookie is mainly used.
  > Let the URL be a `* .json` to distinguish it from the REST API that returns JSON.
- `/pages`: File-based page routing. All ts files in `/pages` are only alias with `export {default}` to `/services/${serviceName}/pages/**`. all implementations should be done inside `/services`.

  ```typescript
  export { default } from '~/services/home/pages/index'
  ```
- `/services`: The application is divided into several services and should be implemented in a folder named by service name. (Example: `/home`, `/auth`, ...)
  - Inside a Service: `/components`, `/queries`, `/pages`, `/helpers`, `/types`, ...
- `/store`: One Store that is globally used.
- `/types`: Declare only `.d.ts`. The type used for each service should be stored in `/types' in each service.

## To-do
- [x] optimize the lambda capacity (create SSR bundle with no dependencies)
- [x] static file serve
- [ ] gzip Compression
