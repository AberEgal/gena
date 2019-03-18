<template>
  <div>
    <h1>Nachhaltigkeit</h1>
    <div v-for="item in profile" :key="item.id">
      <nuxt-link :to="`/article/${item.id}`">
        {{ item.name }}
      </nuxt-link>
    </div>
  </div>
</template>

<script>
import profile from '~/apollo/queries/fetchProfile'
export default {
  apollo: {
    profile: {
      prefetch: true,
      query: profile
    }
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
