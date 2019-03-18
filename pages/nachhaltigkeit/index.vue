<template>
  <div>
    <h1>Nachhaltigkeit</h1>
    <div v-for="item in allPosts" :key="item.id">
      <nuxt-link :to="`/article/${item.id}`">
        {{ item.title }}
        {{ item.body }}
        {{ item.slug }}
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
      title: 'Generation Nachhaltigkeit für mehr Nachhaltigkeit',
      meta: [
        { hid: 'description', name: 'description', content: 'Die Nachhaltigkeitsseite unserer Seite' }
      ]
    }
  }
}
</script>
