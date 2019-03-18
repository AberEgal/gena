<template>
  <div>
    <h1>Nachhaltigkeit</h1>
    <div v-for="item in profiles" :key="item.id">
      <nuxt-link :to="`/article/${item.id}`">
        {{ item.name }}
      </nuxt-link>
    </div>
  </div>
</template>

<script>
import profiles from '~/apollo/queries/fetchProfiles'
export default {
  apollo: {
    profiles: {
      prefetch: true,
      query: profiles
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
