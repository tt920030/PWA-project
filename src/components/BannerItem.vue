<template>
  <div class="banner p-relative mb-5">
    <div class="bg-primary banner__bg"></div>
    <div class="p-absolute w-100 h-100 banner__container container flex-space-between" :class="{'flex-row-reverse': reverse}">
      <div class="banner__picture-container">
        <img class="picture" :src="imgSrc">
      </div>
      <div class="d-flex h-100">
        <div class="banner__content-container">
          <p class="banner__content" v-for="(content, index) in contents" :key="index">
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

<style scoped>
/* .banner {
  padding: 20px 0;

  &__bg {
    height: 420px;
  }

  &__container {
    left: 0;
    top: 0;

    &--reverse {
      flex-direction: row-reverse;
    }
  }

  &__picture-container {
    width: 460px;
    height: 460px;
  }

  &__title {
    margin-left: 80px;
  }

  &__content {
    padding: 90px 0;
    writing-mode: vertical-rl;
    color: $green-200;
    line-height: 2;
  }
} */
</style>
