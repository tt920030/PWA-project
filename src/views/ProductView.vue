<template>
  <div class="product">
    <div class="container mb-5">
      <div class="picture-container p-relative">
        <img
          class="picture"
          src="https://bit.ly/2Qodh3Z"
        >
        <img
          class="p-absolute product__bg-slogan"
          src="@/assets/img/lg-想吃甜點是不需要理由的.png"
        >
      </div>
      <div class="row">
        <nav class="nav col-4">
          <div class="btn-lg bg-secondary flex-center">
            <h2>甜點類別</h2>
          </div>
          <div
            v-for="nav in navList"
            :key="nav.title"
            class="btn-lg flex-center nav__navList"
            :class="{'bg-primary': nowPage === nav.title}"
          >
            <h2>{{ nav.title }}（{{ nav.num }}）</h2>
          </div>
        </nav>
        <div class="col-8">
          <div class="row">
            <div
              v-for="product in products"
              :key="product.name"
              class="col-6 product__card"
            >
              <CardItem
                :imgSrc="product.imgSrc"
                :name="product.name"
                :price="product.price"
                :tag="product.tag"
              />
            </div>
          </div>
        </div>
      </div>
      <div class="d-flex product__pagination">
        <PaginationItem class="mr-0 ml-auto"/>
      </div>
    </div>
  </div>
</template>

<script>
import CardItem from '@/components/CardItem.vue'
import PaginationItem from '@/components/PaginationItem.vue'

export default {
  name: 'ProductView',
  components: {
    CardItem,
    PaginationItem
  },
  data () {
    return {
      navList: [
        { title: '所有甜點', num: 48 },
        { title: '本日精選', num: 10 },
        { title: '人氣推薦', num: 26 },
        { title: '新品上市', num: 12 }
      ],
      nowPage: '所有甜點',
      products: [
        {
          imgSrc: 'https://bit.ly/2QiWeQW',
          name: '焦糖馬卡龍',
          price: 450,
          tag: 1
        },
        {
          imgSrc: 'https://bit.ly/2zBjQuq',
          name: '焦糖馬卡龍2',
          price: 450,
          tag: 1
        },
        {
          imgSrc: 'https://bit.ly/2zKOP7w',
          name: '焦糖馬卡龍3',
          price: 450,
          tag: 1
        },
        {
          imgSrc: 'https://bit.ly/2NcDVuB',
          name: '焦糖馬卡龍4',
          price: 450,
          tag: 1
        },
        {
          imgSrc: 'https://bit.ly/2zBDAxX',
          name: '焦糖馬卡龍5',
          price: 450,
          tag: 1
        },
        {
          imgSrc: 'https://bit.ly/2zL5jN7',
          name: '焦糖馬卡龍6',
          price: 450,
          tag: 1
        }
      ]
    }
  }
}
</script>
