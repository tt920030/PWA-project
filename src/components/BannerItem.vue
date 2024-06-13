<template>
  <div class="banner p-relative mb-5">
    <div class="bg-primary banner__bg"></div>
    <div
      class="
        p-absolute
        w-100
        h-100
        banner__container
        container
        flex-space-between
      "
      :class="{'flex-row-reverse': reverse}"
    >
      <div class="w-50 h-100">
        <img class="picture" :src="imgSrc">
      </div>
      <div class="d-flex h-100">
        <div class="banner__content-container">
          <p
            class="banner__content"
            v-for="(content, index) in contents"
            :key="index"
          >
            {{ content }}
          </p>
        </div>
        <div class="banner__title">
          <img :src="titleSrc">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BannerItem',
  props: {
    imgSrc: {
      type: String,
      required: true
    },
    titleSrc: {
      type: String,
      required: true
    },
    contents: {
      type: Array,
      required: true
    },
    reverse: {
      type: Boolean,
      default: false
    }
  }
}
</script>
