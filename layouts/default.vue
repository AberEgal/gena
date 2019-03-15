<template>
  <div class="container mx-auto px-2 font-sans font-semibold">
    <TheHeader />
    <nuxt class="p-4" />
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader/TheHeader'
import TheFooter from '@/components/TheFooter/TheFooter'

export default {
  components: {
    TheHeader,
    TheFooter
  }
}
</script>

<style>
.nav-link {
  @apply no-underline text-teal-dark text-xl
}

.nav-link:hover {
  @apply underline
}

.footer-link {
  @apply no-underline text-teal-dark text-sm
}

.footer-link:hover {
  @apply underline
}

</style>
