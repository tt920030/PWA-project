<template>
  <div class="card">
    <div class="card__picture-container p-relative">
      <span class="p-absolute material-icons card__like">
        favorite_border
      </span>
      <span v-if="tag" class="p-absolute bg-secondary card__tag">{{ tagText[tag] }}</span>
      <img class="picture" :src=imgSrc>
    </div>
    <div class="flex-center card__info">
      <h3 class="card__info-name h-100 flex-center">{{ name }}</h3>
      <h3 class="card__info-price h-100 flex-center">NT$ {{ price }}</h3>
    </div>
    <button class="btn-lg bg-primary">
      <h2>加入購物車</h2>
    </button>
  </div>
</template>

<script>
export default {
  name: 'CardItem',
  props: {
    imgSrc: {
      type: String,
      required: true
    },
    name: {
      type: String,
      required: true
    },
    price: {
      type: String,
      required: true
    },
    tag: {
      type: Number
    }
  },
  data () {
    return {
      tagText: {
        1: '本日精選',
        2: '人氣推薦',
        3: '新品上市'
      }
    }
  }
}
</script>
