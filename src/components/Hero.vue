<template>
  <section class="hero is-warning is-fullheight is-large is-bold">
      <div class="hero-head">
          <nav class="navbar">
              <div class="container">
                  <div class="navbar-brand">
                      <a class="navbar-item is-large" href="/">
                          Octopus Railways
                      </a>
                  </div>
                  <div id="navbarMenu" class="navbar-menu" :class="{'is-active': navActive}">
                      <div class="navbar-end">
                          <div class="tabs is-center">
                              <ul>
                                  <li class="is-active"><a>Home</a></li>
                                  <li><a href="">Operating Lines</a></li>
                                  <li><a href="">Team</a></li>
                              </ul>
                              <span class="navbar-item">
                                  <a class="button is-black is-outlined" href="/">
                                      <span title="log in">log in</span>
                                  </a>
                              </span>
                          </div>
                      </div>
                  </div>
                <a role="button" class="navbar-burger" data-target="navbarMenu" :class="{'is-active': navActive}" @click="toggleMenu">
                  <span></span>
                  <span></span>
                  <span></span>
                </a>
              </div>
          </nav>
      </div>
      <div class="hero-body">
        <div class="container columns">
          <app-search-form class="column is-6 is-offset-1"></app-search-form>
          <div class="column is-3 is-offset-3">
            <img src="../assets/octopus.svg" id="logo" alt="Logo">
          </div>          
        </div>
      </div>
  </section>
</template>

<script>
import SearchForm from './SearchForm'
export default {
  components: {
    appSearchForm: SearchForm
  },
  data() {
    return {
      navActive: false
    }
  },
  methods: {
    toggleMenu() {
      this.navActive = !this.navActive
    }
  }
  
}
</script>


<style lang="scss" scoped>

#logo {
  max-width: 100%;
  height: auto;
}

</style>
