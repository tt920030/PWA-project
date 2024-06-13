<template>
  <ul class="pagination d-flex">
    <li class="pagination__item flex-center">
      <span class="material-icons">arrow_left</span>
    </li>
    <li
      v-for="i in 3"
      :key="i"
      class="pagination__item flex-center"
      :class="{'bg-secondary': nowPage === i}"
    >
      {{ i }}
    </li>
    <li class="pagination__item flex-center">
      <span class="material-icons">arrow_right</span>
    </li>
  </ul>
</template>

<script>
export default {
  name: 'PaginationItem',
  props: {
    nowPage: {
      type: Number,
      default: 1
    }
  }
}
</script>
