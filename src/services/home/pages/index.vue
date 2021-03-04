<template>
  <div>
  <section class="hero main-hero is-medium is-bold">
    <div class="hero-head">
      <nav class="navbar">
        <div class="container">
          <div class="navbar-brand">
            <a class="navbar-item" href="/">
              <img src="/static/pachamama-logo.png" alt="Logo">
            </a>
            <span class="navbar-burger burger" data-target="navbarMenu">
                                <span></span>
                                <span></span>
                                <span></span>
                            </span>
          </div>
          <div id="navbarMenu" class="navbar-menu">
            <div class="navbar-end">
              <div class="tabs is-right">
                <div class="buttons">
                  <a class="button is-primary">
                    <strong>Sign up</strong>
                  </a>
                  <a class="button is-light">
                    Log in
                  </a>
                  <a class="button is-light">
                   Explore
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </nav>
    </div>
    <div class="hero-body">
      <div class="container has-text-centered">
        <h1 class="title">
          Pachamama
        </h1>
        <h2 class="subtitle">
          Pachamama est une application que te permettra de créer facilement et rapidement ton propre carnet de voyage en ligne.
        </h2>
      </div>
    </div>
  </section>
  <div class="box cta">
    <p class="has-text-centered">
      <span class="tag is-primary">Cooming soon</span> L'application est en cours de developpement.
    </p>
  </div>
  <section class="container">
    <div class="columns features">
      <div class="column is-4">
        <div class="card is-shady">
          <div class="card-image has-text-centered">
            <i class="fa fa-paw"></i>
          </div>
          <div class="card-content">
            <div class="content">
              <h4>This is a content test. </h4>
              <p>Purus semper eget duis at tellus at urna condimentum mattis. Non blandit massa enim nec. Integer enim neque volutpat ac tincidunt vitae semper quis. Accumsan tortor posuere ac ut consequat semper viverra nam.</p>
              <p><a href="#">Learn more</a></p>
            </div>
          </div>
        </div>
      </div>
      <div class="column is-4">
        <div class="card is-shady">
          <div class="card-image has-text-centered">
            <i class="fa fa-empire"></i>
          </div>
          <div class="card-content">
            <div class="content">
              <h4>Tempor orci dapibus ultrices in.</h4>
              <p>Ut venenatis tellus in metus vulputate. Amet consectetur adipiscing elit pellentesque. Sed arcu non odio euismod lacinia at quis risus. Faucibus turpis in eu mi bibendum neque egestas cmonsu songue. Phasellus vestibulum lorem
                sed risus.</p>
              <p><a href="#">Learn more</a></p>
            </div>
          </div>
        </div>
      </div>
      <div class="column is-4">
        <div class="card is-shady">
          <div class="card-image has-text-centered">
            <i class="fa fa-apple"></i>
          </div>
          <div class="card-content">
            <div class="content">
              <h4> Leo integer malesuada nunc vel risus. </h4>
              <p>Imperdiet dui accumsan sit amet nulla facilisi morbi. Fusce ut placerat orci nulla pellentesque dignissim enim. Libero id faucibus nisl tincidunt eget nullam. Commodo viverra maecenas accumsan lacus vel facilisis.</p>
              <p><a href="#">Learn more</a></p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="intro column is-8 is-offset-2">
      <h2 class="title">Perfect for developers or designers!</h2><br>
      <p class="subtitle">Vel fringilla est ullamcorper eget nulla facilisi. Nulla facilisi nullam vehicula ipsum a. Neque egestas congue quisque egestas diam in arcu cursus.</p>
    </div>
    <div class="sandbox">
      <div class="tile is-ancestor">
        <div class="tile is-parent is-shady">
          <article class="tile is-child notification is-white">
            <p class="title">Hello World</p>
            <p class="subtitle">What is up?</p>
          </article>
        </div>
        <div class="tile is-parent is-shady">
          <article class="tile is-child notification is-white">
            <p class="title">Foo</p>
            <p class="subtitle">Bar</p>
          </article>
        </div>
        <div class="tile is-parent is-shady">
          <article class="tile is-child notification is-white">
            <p class="title">Third column</p>
            <p class="subtitle">With some content</p>
            <div class="content">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin ornare magna eros, eu pellentesque tortor vestibulum ut. Maecenas non massa sem. Etiam finibus odio quis feugiat facilisis.</p>
            </div>
          </article>
        </div>
      </div>
      <div class="tile is-ancestor">
        <div class="tile is-vertical is-8">
          <div class="tile">
            <div class="tile is-parent is-vertical">
              <article class="tile is-child notification is-white">
                <p class="title">Vertical tiles</p>
                <p class="subtitle">Top box</p>
              </article>
              <article class="tile is-child notification is-white">
                <p class="title">Vertical tiles</p>
                <p class="subtitle">Bottom box</p>
              </article>
            </div>
            <div class="tile is-parent">
              <article class="tile is-child notification is-white">
                <p class="title">Middle box</p>
                <p class="subtitle">With an image</p>
                <figure class="image is-4by3">
                  <img src="https://picsum.photos/640/480/?random" alt="Description">
                </figure>
              </article>
            </div>
          </div>
          <div class="tile is-parent is-shady">
            <article class="tile is-child notification is-white">
              <p class="title">Wide column</p>
              <p class="subtitle">Aligned with the right column</p>
              <div class="content">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin ornare magna eros, eu pellentesque tortor vestibulum ut. Maecenas non massa sem. Etiam finibus odio quis feugiat facilisis.</p>
              </div>
            </article>
          </div>
        </div>
        <div class="tile is-parent is-shady">
          <article class="tile is-child notification is-white">
            <div class="content">
              <p class="title">Tall column</p>
              <p class="subtitle">With even more content</p>
              <div class="content">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at pulvinar felis blandit. Vestibulum volutpat tellus diam, consequat gravida libero rhoncus ut. Morbi maximus, leo sit amet vehicula
                  eleifend, nunc dui porta orci, quis semper odio felis ut quam.</p>
                <p>Suspendisse varius ligula in molestie lacinia. Maecenas varius eget ligula a sagittis. Pellentesque interdum, nisl nec interdum maximus, augue diam porttitor lorem, et sollicitudin felis neque sit amet erat. Maecenas imperdiet
                  felis nisi, fringilla luctus felis hendrerit sit amet. Aenean vitae gravida diam, finibus dignissim turpis. Sed eget varius ligula, at volutpat tortor.</p>
                <p>Integer sollicitudin, tortor a mattis commodo, velit urna rhoncus erat, vitae congue lectus dolor consequat libero. Donec leo ligula, maximus et pellentesque sed, gravida a metus. Cras ullamcorper a nunc ac porta. Aliquam
                  ut aliquet lacus, quis faucibus libero. Quisque non semper leo.</p>
              </div>
            </div>
          </article>
        </div>
      </div>
      <div class="tile is-ancestor">
        <div class="tile is-parent is-shady">
          <article class="tile is-child notification is-white">
            <p class="title">Side column</p>
            <p class="subtitle">With some content</p>
            <div class="content">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin ornare magna eros, eu pellentesque tortor vestibulum ut. Maecenas non massa sem. Etiam finibus odio quis feugiat facilisis.</p>
            </div>
          </article>
        </div>
        <div class="tile is-parent is-8 is-shady">
          <article class="tile is-child notification is-white">
            <p class="title">Main column</p>
            <p class="subtitle">With some content</p>
            <div class="content">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin ornare magna eros, eu pellentesque tortor vestibulum ut. Maecenas non massa sem. Etiam finibus odio quis feugiat facilisis.</p>
            </div>
          </article>
        </div>
      </div>
      <div class="tile is-ancestor">
        <div class="tile is-parent is-8 is-shady">
          <article class="tile is-child notification is-white">
            <p class="title">Murphy's law</p>
            <p class="subtitle">Anything that can go wrong will go wrong</p>
            <div class="content">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin ornare magna eros, eu pellentesque tortor vestibulum ut. Maecenas non massa sem. Etiam finibus odio quis feugiat facilisis.</p>
            </div>
          </article>
        </div>
        <div class="tile is-parent is-shady">
          <article class="tile is-child notification is-white">
            <p class="title">Main column</p>
            <p class="subtitle">With some content</p>
            <div class="content">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin ornare magna eros, eu pellentesque tortor vestibulum ut. Maecenas non massa sem. Etiam finibus odio quis feugiat facilisis.</p>
            </div>
          </article>
        </div>
      </div>
    </div>
  </section>
  <footer class="footer">
    <div class="container">
      <div class="columns">
        <div class="column is-3 is-offset-2">
          <h2><strong>Category</strong></h2>
          <ul>
            <li><a href="#">Lorem ipsum dolor sit amet</a></li>
            <li><a href="#">Vestibulum errato isse</a></li>
            <li><a href="#">Lorem ipsum dolor sit amet</a></li>
            <li><a href="#">Aisia caisia</a></li>
            <li><a href="#">Murphy's law</a></li>
            <li><a href="#">Flimsy Lavenrock</a></li>
            <li><a href="#">Maven Mousie Lavender</a></li>
          </ul>
        </div>
        <div class="column is-3">
          <h2><strong>Category</strong></h2>
          <ul>
            <li><a href="#">Labore et dolore magna aliqua</a></li>
            <li><a href="#">Kanban airis sum eschelor</a></li>
            <li><a href="#">Modular modern free</a></li>
            <li><a href="#">The king of clubs</a></li>
            <li><a href="#">The Discovery Dissipation</a></li>
            <li><a href="#">Course Correction</a></li>
            <li><a href="#">Better Angels</a></li>
          </ul>
        </div>
        <div class="column is-4">
          <h2><strong>Category</strong></h2>
          <ul>
            <li><a href="#">Objects in space</a></li>
            <li><a href="#">Playing cards with coyote</a></li>
            <li><a href="#">Goodbye Yellow Brick Road</a></li>
            <li><a href="#">The Garden of Forking Paths</a></li>
            <li><a href="#">Future Shock</a></li>
          </ul>
        </div>
      </div>
      <div class="content has-text-centered">
        <p>
          <a class="icon" href="https://github.com/BulmaTemplates/bulma-templates">
            <i class="fa fa-github"></i>
          </a>
        </p>
        <div class="control level-item">
          <a href="https://github.com/BulmaTemplates/bulma-templates">
            <div class="tags has-addons">
              <span class="tag is-dark">Bulma Templates</span>
              <span class="tag is-info">MIT license</span>
            </div>
          </a>
        </div>
      </div>
    </div>
  </footer>
  </div>
</template>
<style lang="scss">
// Import Bulma's core
@import "../../../scss/app.scss";
</style>

<script lang='ts'>
import {Component, Vue} from 'nuxt-property-decorator'
import {State} from 'vuex-class'
import {IEnvironments} from '~/store'

@Component
export default class PageIndex extends Vue {
  @State((state) => state.environments)
  environments: IEnvironments

  /**
   * You can fetch data from remote server with 'asyncData()' method
   */
  async asyncData() {
    return {
      message: 'Comming soon',
    }
  }

  /**
   * overide tags in <head> with 'head()' method
   */
  head() {
    return {
      title: 'Pachama travel - coming soon',
    }
  }
}
</script>

<style lang='scss'>
.page-index {
  h1 {
    color: #087f5b;
  }
}
</style>
