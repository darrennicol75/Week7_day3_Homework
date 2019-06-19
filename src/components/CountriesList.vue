<template lang="html">
  <div>
    <ul>
      <country-item v-for="(country, index) in countries" :country="country" :key="index"></country-item>
    </ul>
  </div>
</template>

<script>
import CountryItem from './CountryItem.vue'

export default {
  name: 'country-list',
  props: ['countries'],
  components: {
    "country-item": CountryItem
  }
}
</script>

<style lang="css" scoped>
</style>
