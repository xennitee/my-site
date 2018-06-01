<template>
  <div class="content-index-list">
    <ContentIndexListItem
      v-for="item in indexList"
      v-bind:key="item.id"
      v-bind:item="item"
    />
  </div>
</template>

<script>
import ContentIndexListItem from '../components/ContentIndexListItem.vue'

export default {
  name: 'ContentIndexList',
  components: {
    ContentIndexListItem
  },
  data () {
    return {
      indexList: [
        {id: 0, text: '0.0.0.0.0.0.', bookmark: '#contact'},
        {id: 1, text: '1.1.1.1.1.1.', bookmark: '#experience'},
        {id: 2, text: '2.2.2.2.2.2.', bookmark: '#education'}
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
a {
  font-size: 20px;
}
</style>
