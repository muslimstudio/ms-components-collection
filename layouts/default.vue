<template>
  <div>
    <Header :darkMode="darkMode" @toggle-dark-mode="darkMode = $event" />
    <div></div>
    <Canvas>
      <Nuxt />
    </Canvas>
  </div>
</template>
<script>
import Header from '~/components/global/Header'
import Canvas from '~/components/global/Canvas'
export default {
  components: {
    Header,
    Canvas
  },
  data () {
    return {
      darkMode: false
    }
  },
  watch: {
    darkMode (value) {
      this.$colorMode.preference = value
      this.darkMode = value
      // localStorage.setItem('tcvDarkMode', value)
    }
  },
  mounted () {
    this.darkMode = localStorage.getItem('tcvDarkMode') === 'true'
    this.$colorMode.preference = localStorage.getItem('tcvDarkMode') === 'true'
  }
}
</script>