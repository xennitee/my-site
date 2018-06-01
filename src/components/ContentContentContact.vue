<template>
  <p>
    {{contactme.name}}<br />
    {{contactme.location}}<br />
    {{contactme.phone}}<br />
    {{contactme.email}}<br />
  </p>
</template>

<script>
export default {
  name: 'ContentContentContact',
  props: {
    contactme: {
      type: Object
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p {
  text-align: right;
}
</style>
