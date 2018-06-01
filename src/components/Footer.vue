<template>
  <div class="footer">
    <h5>{{ copyright }}</h5>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    copyright: {
      type: String
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  background-color: #BBBBBB;
  padding: 10px;
}
</style>
