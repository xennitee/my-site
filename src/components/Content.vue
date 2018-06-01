<template>
  <div class="content">
    <ContentIndexList class="menu"/>
    <ContentContent class="content-content"/>
  </div>
</template>

<script>
import ContentIndexList from '../components/ContentIndexList.vue'
import ContentContent from '../components/ContentContent.vue'

export default {
  name: 'Content',
  components: {
    ContentIndexList,
    ContentContent
  },
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.content {
  display: flex;
  flex-wrap: wrap;
}
.menu {
  flex: 30%;
}
.content-content {
  flex: 70%;
}
</style>
