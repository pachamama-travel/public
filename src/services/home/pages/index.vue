<template>
  <div>
  <section class="hero main-hero is-medium is-bold">
    <div class="hero-head">
      <nav class="navbar">
        <div class="container">
          <div class="navbar-brand">
            <a class="navbar-item" href="/">
              <img src="/static/pachamama-logo.png" alt="Logo">
              <img src="/static/logo-icon.png" alt="Logo">
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
        <h1 class="subtitle">
          Discover the World, Create your Travel Diary and Share your Experiences!
        </h1>
      </div>
    </div>
  </section>
  <div class="box cta">
    <p class="has-text-centered">
      <span class="tag is-primary">Cooming soon</span> Application in progress
    </p>
  </div>
  <section class="container home-cards">
    <div class="columns features">
      <div class="column is-4">
        <div class="card is-shady">
          <div class="card-image has-text-centered">
            <i class="fa fa-paw"></i>
          </div>
          <div class="card-content">
            <div class="content has-text-centered">
              <h3>Travel with Responsibility and be a more Sustainable Traveler 🌿 </h3>
            </div>
          </div>
        </div>
      </div>
      <div class="column is-4">
        <div class="card is-shady">
          <div class="card-image has-text-centered">
            <i class="fa fa-empire"></i>
          </div>
          <div class="card-content" style="margin-top: 20px;">
            <div class="content has-text-centered">
              <h3>Support Local Tourism 🏕</h3>
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
            <div class="content has-text-centered">
              <h3>Create your Travel Diary and Share your Experiences 🌍. </h3>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <footer class="footer">
    <div class="container">
      <div class="columns">
        <div class="column is-3 is-offset-2">
          <h2><strong>Pages</strong></h2>
          <ul>
            <li><a href="/">Home</a></li>
          </ul>
        </div>
      </div>
      <div class="content has-text-centered">
        <div class="control level-item">
          Pachamama 2021
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
