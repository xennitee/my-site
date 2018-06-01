<template>
  <div class="content-content">
    <ContentContentContact v-bind:contactme="resume.contact"/>
    <h3>{{resume.titleExp}}</h3>
    <ContentContentExpItem
      v-for="item in resume.exp"
      v-bind:key="resume.exp.indexOf(item)"
      v-bind:items="item"
    />
    <h3>{{resume.titleEdu}}</h3>
    <ContentContentExpItem
      v-for="item in resume.edu"
      v-bind:key="resume.edu.indexOf(item) + 1"
      v-bind:items="item"
    />
  </div>
</template>

<script>
import ContentContentContact from '../components/ContentContentContact.vue'
import ContentContentExpItem from '../components/ContentContentExpItem.vue'

export default {
  name: 'ContentContent',
  components: {
    ContentContentContact,
    ContentContentExpItem
  },
  data () {
    return {
      resume: {
        contact: {
          name: 'Chia-Hsu Chen (Reno Chen)',
          location: 'Monterey Park, CA',
          phone: 'xxx xxx xxxx',
          email: 'xennitee.u@gmail.com'
        },
        titleExp: 'titleExp',
        exp: [
          {
            when: 'when',
            where: 'where',
            what: 'what',
            how: [
              {idx: 0, content: 'content'},
              {idx: 1, content: 'content'}
            ]
          }
        ],
        titleEdu: 'titleEdu',
        edu: [
          {
            when: 'when',
            where: 'where',
            what: 'what',
            how: [
              {idx: 0, content: 'content'},
              {idx: 1, content: 'content'}
            ]
          },
          {
            when: 'when',
            where: 'where',
            what: 'what',
            how: [
            ]
          }
        ]
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  text-align: left;
}
</style>
