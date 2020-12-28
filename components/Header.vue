<template>
  <div class="placeholder">
    <div class="window">
      <div class="tm-header">
        <div class="row tm-header-inner">
          <div class="col-md-6 col-12">
            <img src="~assets/images/logo-evermos.jpg" alt="Logo" class="tm-site-logo" style="border-radius: 10px;" />
            <div class="tm-site-text-box">
              <h1 class="tm-site-title">
                Evermos Shopping
              </h1>
              <h6 class="tm-site-description">
                new shopping modern
              </h6>
            </div>
          </div>
          <nav class="col-md-6 col-12 tm-nav">
            <ul class="tm-nav-ul">
              <li class="tm-nav-li">
                <a @click="directToIndex" class="tm-nav-link active">Home</a>
              </li>
              <li class="tm-nav-li">
                <a @click="directToAbout" class="tm-nav-link">About</a>
              </li>
              <li class="tm-nav-li">
                <a @click="directToRegister" class="tm-nav-link">Register</a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      dialog: false,
      title: null,
      content: null,
      message: null
    }
  },
  methods: {
    directToAbout () {
      this.$router.push('/about/about')
    },
    directToIndex () {
      this.$router.push('/')
    },
    directToRegister () {
      window.open('https://lp.evermos.com/daftar-reseller-evermos-juragan/?utm_source=adwords&utm_medium=ppc&utm_term=peluang')
    }
  }
}
</script>

<style>

</style>
