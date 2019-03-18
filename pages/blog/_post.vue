<template>
  <div>
    <h1>Dies ist ein Post mit der URL {{ this.$route.params.post }} </h1>
    <div v-for="item in singlePost" :key="item.id">
      {{ item.title }}
    </div>
  </div>
</template>

<script>
import gql from 'graphql-tag'
export default {
  apollo: {
    singlePost: {
      query: gql`query {
        singlePost(url: "post_3_zum_sieg") {
          title
          body
          updatedAt
        }
      }`,
      prefetch: ({ route }) => ({ id: route.params.post }),
      variables() {
        return { url: this.$route.params.post }
      }
    }
  },
  head() {
    return {
      title: 'Ein bestimmtes Posting',
      meta: [
        { hid: 'description', name: 'description', content: 'Ein Posting unserers Blogs' }
      ]
    }
  }
}
</script>
