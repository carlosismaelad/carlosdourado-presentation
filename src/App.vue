<template>
  <header>
    <TheHeader/>
    <GroupSections/>
  </header>
</template>


<script>
import './assets/main.css'
import TheHeader from './components/header/TheHeader.vue'
import GroupSections from './components/sections/GroupSections.vue'

export default {
  name: 'App',
  components: {
    TheHeader,
    GroupSections,
  }
}
</script>


<style scoped>
h2{
  color: #00ffe9;
}

</style>
