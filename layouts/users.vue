<template>
  <div>
    <Header /> <!-- imported Component -->
    <p> This header is coming from the Header component which is imported into the users.uve Layout</p>
    <nuxt/>
  </div>
</template>

<script>
import Header from '~/components/Header.vue'

export default {
  components: {
   Header
  }
}
</script>

<style>

</style>
