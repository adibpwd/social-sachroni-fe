<template>
  <div>
     <header>
      <nav class="navbar is-transparent">
        <div class="navbar-brand">
          <a class="navbar-item" href="https://bulma.io">
            <img src="https://bulma.io/images/bulma-logo.png" alt="Bulma: a modern CSS framework based on Flexbox"
              width="112" height="28">
          </a>
          <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" @click="isOpen = !isOpen" v-bind:class="{'is-active': isOpen}">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div id="navbarExampleTransparentExample" class="navbar-menu" v-bind:class="{'is-active': isOpen}">
          <div class="navbar-start" style="flex-grow: 1; justify-content: center;">
            <a class="navbar-item" href="https://bulma.io/">
              Home
            </a>
            <div class="navbar-item has-dropdown is-hoverable">
              <a class="navbar-link" href="https://bulma.io/documentation/overview/start/">
                Docs
              </a>
              <div class="navbar-dropdown is-boxed">
                <a class="navbar-item" href="https://bulma.io/documentation/overview/start/">
                  Overview
                </a>
                <a class="navbar-item" href="https://bulma.io/documentation/overview/modifiers/">
                  Modifiers
                </a>
                <a class="navbar-item" href="https://bulma.io/documentation/columns/basics/">
                  Columns
                </a>
                <a class="navbar-item" href="https://bulma.io/documentation/layout/container/">
                  Layout
                </a>
                <a class="navbar-item" href="https://bulma.io/documentation/form/general/">
                  Form
                </a>
                <hr class="navbar-divider">
                <a class="navbar-item" href="https://bulma.io/documentation/elements/box/">
                  Elements
                </a>
                <a class="navbar-item is-active" href="https://bulma.io/documentation/components/breadcrumb/">
                  Components
                </a>
              </div>
            </div>
          </div>

          <div class="navbar-end">
            <div class="navbar-item">
              <div class="field is-grouped">
                <p class="control">
                  <a class="bd-tw-button button" data-social-network="Twitter" data-social-action="tweet"
                    data-social-target="https://bulma.io" target="_blank"
                    href="https://twitter.com/intent/tweet?text=Bulma: a modern CSS framework based on Flexbox&amp;hashtags=bulmaio&amp;url=https://bulma.io&amp;via=jgthms">
                    <span class="icon">
                      <!-- <font-awesome-icon :icon="['fas', 'lock']"/> -->
                      <!-- <i class="fab fa-twitter"></i> -->
                    </span>
                    <span>
                      Tweet
                    </span>
                  </a>
                </p>
                <p class="control">
                  <a class="button is-primary"
                    href="https://github.com/jgthms/bulma/releases/download/0.9.4/bulma-0.9.4.zip">
                    <span class="icon">
                      <i class="fas fa-download"></i>
                    </span>
                    <span>Download</span>
                  </a>
                </p>
              </div>
            </div>
          </div>
        </div>
      </nav>
    </header>
    Some shared layout content:
    <slot />
    <footer>

    </footer>
  </div>
</template>

<script>
  export default {
    data: function(){
      return {
        isOpen: false
      }
    }
  }
</script>

<style>
</style>