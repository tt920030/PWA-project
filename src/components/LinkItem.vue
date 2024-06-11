<template>
  <router-link :to="to" class="col-3 linkItem__container p-relative">
    <div class="p-absolute linkItem__link">
      <h2 class="flex-center w-100">{{ text }}</h2>
    </div>
  </router-link>
</template>

<script>
export default {
  props: {
    to: {
      type: String,
      required: true
    },
    text: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
/* 你的樣式 */
</style>
