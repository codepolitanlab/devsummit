<template>
  <div>
    <div class="navbar-group" :class="{ 'hidden-navbar': !showNavbar }">
      <div ref="cpNavbarGroup">
        <b-navbar toggleable="lg" type="light" variant="white" class="flex-column">
          <b-container>
            <b-navbar-brand to="/">
              <img src="/img/codepolitan.png" alt="codepolitan">
            </b-navbar-brand>

            <b-navbar-toggle target="navbar-toggle-collapse">
              <template #default="{ expanded }">
                <b-icon v-if="expanded" icon="chevron-bar-up" />
                <b-icon v-else icon="chevron-bar-down" />
              </template>
            </b-navbar-toggle>

            <b-collapse id="navbar-toggle-collapse" is-nav>
              <b-navbar-nav class="ml-auto pb-md-0">
                <b-nav-item-dropdown
                  id="my-nav-dropdown"
                  text="program belajar"
                  toggle-class="nav-link ml-3 nav-text text-uppercase"
                  class="my-1"
                >
                  <b-dropdown-item target="_blank" :href="link + 'library'">
                    Semua Kelas
                  </b-dropdown-item>
                  <b-dropdown-item target="_blank" :href="link + 'library'">
                    Kelas Android
                  </b-dropdown-item>
                  <b-dropdown-item class="mr-5 pr-5" target="_blank" :href="link + 'library'">
                    Kelas Web Development
                  </b-dropdown-item>
                  <b-dropdown-item target="_blank" :href="link + 'library'">
                    Kelas CodeIgniter
                  </b-dropdown-item>
                  <b-dropdown-item target="_blank" :href="link + 'library'">
                    Kelas Laravel
                  </b-dropdown-item>
                  <b-dropdown-item target="_blank" :href="link + 'library'">
                    Kelas JavaScript
                  </b-dropdown-item>
                  <b-dropdown-item target="_blank" :href="link + 'library'">
                    Kelas Gratis
                  </b-dropdown-item>
                  <b-dropdown-divider class="mt-3 mb-3" />
                  <b-dropdown-item target="_blank" href="https://devschool.id/">
                    Developer School
                  </b-dropdown-item>
                  <!-- <b-dropdown-item to="/fullstack">Full Stack Developer</b-dropdown-item> -->
                  <b-dropdown-item target="_blank" href="https://kampuscoding.id/" class="d-flex">
                    <div class="d-flex align-items-center">
                      Kampus Coding
                    </div>
                  </b-dropdown-item>
                  <b-dropdown-item target="_blank" href="https://programmerzamannow.codepolitan.com/" class="d-flex">
                    <div class="d-flex align-items-center">
                      Programmer Zaman Now <b-badge class="ml-auto" variant="danger">
                        NEW
                      </b-badge>
                    </div>
                  </b-dropdown-item>
                  <!-- <b-dropdown-divider class="mt-3 mb-3"></b-dropdown-divider> -->
                </b-nav-item-dropdown>
                <a class="nav-link my-1 ml-3 nav-text text-uppercase" :href="link + 'articles'">
                  Articles
                </a>
                <a class="nav-link my-1 ml-3 nav-text text-uppercase" :href="link + 'forum'">
                  Forum
                </a>
                <a class="nav-link my-1 ml-3 nav-text text-uppercase" :href="link + 'membership'">
                  Premium
                </a>
                <div class="my-1">
                  <a :href="login" class="btn ml-3 btn-light text-dark nav-link type--bold text-uppercase px-3">Login</a>
                </div>
                <div class="my-1">
                  <a :href="register" class="btn ml-3 btn--primary text-white nav-link type--bold text-uppercase px-3">Register</a>
                </div>
              </b-navbar-nav>
            </b-collapse>
          </b-container>
        </b-navbar>
      </div>
    </div>
    <div :style="{height: ( cpNavbarGroupHeight + 10) + 'px', position: 'relative'}" />
  </div>
</template>

<script>
const OFFSET = 60
export default {
  data () {
    return {
      login: 'https://apps.codepolitan.com/user/login',
      register: 'https://apps.codepolitan.com/user/register',
      showNavbar: true,
      lastScrollPosition: 0,
      scrollValue: 0,
      cpNavbarGroupHeight: 0,
      showDismissablePromo: true,
      link: 'https://www.codepolitan.com/'
    }
  },
  mounted () {
    this.lastScrollPosition = window.pageYOffset
    window.addEventListener('scroll', this.onScroll)
    const viewportMeta = document.createElement('meta')
    viewportMeta.name = 'viewport'
    viewportMeta.content = 'width=device-width, initial-scale=1'
    document.head.appendChild(viewportMeta)
    this.cpNavbarGroupHeight = this.$refs.cpNavbarGroup.offsetHeight
  },
  beforeDestroy () {
    window.removeEventListener('scroll', this.onScroll)
  },
  methods: {
    onScroll () {
      if (window.pageYOffset < 0) {
        return
      }
      if (Math.abs(window.pageYOffset - this.lastScrollPosition) < OFFSET) {
        return
      }
      this.showNavbar = window.pageYOffset < this.lastScrollPosition
      this.lastScrollPosition = window.pageYOffset
    },
    dismissPromo () {
      this.showDismissablePromo = false
      this.cpNavbarGroupHeight = this.$refs.cpNavbarGroup.offsetHeight - this.$refs.banner.offsetHeight
    }
  }
}
</script>

<style scoped>
.nav-text {
  color: #707070;
}
span {
  font-weight: bold;
}
.text-membership {
  color: #ffffff !important;
}
.btn--primary {
  border-radius: 0.65rem;
}
ul:not([class*='menu']) li > a {
  font-weight: bold !important;
}
.dropdown-menu .show {
  width: 30vw;
}
#my-nav-dropdown__BV_toggle_ span {
  font-weight: bold !important
}
#banner {
  /* background-color: #E67E22; */
  background-color: #f50057;
  color: #FFFFFF;
}
.navbar-group {
  position: fixed;
  width: 100%;
  z-index: 1050;
  transform: translate3d(0, 0, 0);
  transition: 0.5s all ease-out;
  box-shadow: 0 2px 15px rgba(71, 120, 120, 0.5);
}
.navbar-group.hidden-navbar {
  transform: translate3d(0, -100%, 0);
  box-shadow: none;
}
</style>
