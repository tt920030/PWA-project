<template>
  <HeaderLayout></HeaderLayout>
  <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav> -->
  <router-view/>
</template>

<script>
import HeaderLayout from '@/layout/HeaderLayout'

export default {
  components: {
    HeaderLayout
  }
}
</script>
