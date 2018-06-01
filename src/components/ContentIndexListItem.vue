<template>
  <div class="content-index-list-item">
    <a v-bind:href="item.bookmark">
      {{item.text}}
    </a>
  </div>
</template>

<script>
export default {
  name: 'ContentIndexListItem',
  props: {
    item: {
      type: Object
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  margin: 10px;
}
a {
  font-size: 20px;
}
</style>
