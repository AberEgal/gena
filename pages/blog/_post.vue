<template>
  <h1>Dies ist ein Post!</h1>
</template>

<script>
export default {
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
