<template>
  <div class="list flex-space-between">
    <div class="list__picture-container">
      <img class="picture" :src="imgSrc">
    </div>
    <div class="list__info">
      <h3 class="list__text">{{ name }}</h3>
      <h3 class="list__text">NT$ {{ price }}</h3>
    </div>
    <div class="d-flex">
      <button class="list__btn list__btn--hover flex-center">-</button>
      <span class="list__btn flex-center">1</span>
      <button class="list__btn list__btn--hover flex-center">+</button>
    </div>
    <div class="list__total">
      <h3>NT$ 900</h3>
    </div>
    <span class="list__delete material-icons">
      delete_outline
    </span>
  </div>
</template>

<script>
export default {
  name: 'ListItem',
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
    }
  }
}
</script>
