<template>
  <div>
    <h1>Nachhaltigkeit</h1>
    <div v-for="item in allPosts" :key="item.id">
      <nuxt-link :to="`/blog/${item.url}`">
        {{ item.title }}
      </nuxt-link>
    </div>
  </div>
</template>

<script>
import allPosts from '~/apollo/queries/allPosts'
export default {
  apollo: {
    allPosts
  },
  head() {
    return {
      title: 'Die Blogstartseite',
      meta: [
        { hid: 'description', name: 'description', content: 'Die Startseite unserers Blogs' }
      ]
    }
  }
}
</script>
