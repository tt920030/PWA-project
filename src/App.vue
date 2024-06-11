<template>
  <HeaderLayout />
  <router-view/>
  <FooterLayout />
</template>

<script>
import HeaderLayout from '@/layout/HeaderLayout'
import FooterLayout from '@/layout/FooterLayout'

export default {
  components: {
    HeaderLayout,
    FooterLayout
  }
}
</script>
