<template>
  <div>
    <p>
      {{items.when}}<br />
      {{items.where}}<br />
      {{items.what}}
    </p>
    <ul>
      <li
        v-for="item in items.how"
        v-bind:key="item.idx"
      >
        {{item.content}}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'ContentContentExpItem',
  props: {
    items: {
      type: Object
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p {
  font-weight: bold;
}
</style>
