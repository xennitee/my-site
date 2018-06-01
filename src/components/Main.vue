<template>
  <div class="Main">
    <Header v-bind:title="titleText"/>
    <Content/>
    <Footer v-bind:copyright="copyrightText"/>
  </div>
</template>

<script>
import Header from '../components/Header.vue'
import Content from '../components/Content.vue'
import Footer from '../components/Footer.vue'

export default {
  name: 'Main',
  components: {
    Header,
    Content,
    Footer
  },
  data () {
    return {
      titleText: 'My Profile',
      copyrightText: 'Copyright © No Copyright'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
