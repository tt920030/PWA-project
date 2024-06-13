<template>
  <div class="cart container mb-5">
    <div class="row">
      <div class="col-8">
        <h2 class="cart__title bg-primary text-center">您的購物車</h2>
        <template v-for="list in lists" :key="list.name">
          <ListItem
            :imgSrc="list.imgSrc"
            :name="list.name"
            :price="list.price"
          />
        </template>
      </div>
      <div class="col-4">
        <div class="order-sum bg-secondary">
          <h3 class="order-sum__title text-center">訂單摘要</h3>
          <div class="order-sum__line flex-space-between">
            <p>小計</p><p>NT$ 2,700</p>
          </div>
          <div class="order-sum__line flex-space-between">
            <p>運費</p><p>NT$ 300</p>
          </div>
          <div class="order-sum__total flex-space-between">
            <h3>總計</h3><h3>NT$ 3,000</h3>
          </div>
        </div>
        <router-link to="/checkout">
          <button class="btn-lg bg-tertiary">
            <h2>結帳</h2>
          </button>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
import ListItem from '@/components/ListItem.vue'

export default {
  name: 'CartView',
  components: {
    ListItem
  },
  data () {
    return {
      lists: [
        {
          imgSrc: 'https://bit.ly/2zBDAxX',
          name: '焦糖馬卡龍',
          price: '450'
        },
        {
          imgSrc: 'https://bit.ly/2QvsT63',
          name: '焦糖',
          price: '4500'
        },
        {
          imgSrc: 'https://bit.ly/2QvsT63',
          name: '焦糖馬卡',
          price: '4500'
        }
      ]
    }
  }
}
</script>
