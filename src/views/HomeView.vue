<template>
  <div class="home">
    <div class="container">
      <div class="
        picture-container
        p-relative
        home__picture-container
      ">
        <img
          class="picture"
          src="https://bit.ly/2OhbMHr"
        >
        <div class="
          row
          justify-content-center
          p-absolute
          w-100
          home__links
        ">
          <LinkItem to="/product" text="本日精選" class="home__link--1" />
          <LinkItem to="/product" text="人氣推薦" class="home__link--2" />
          <LinkItem to="/product" text="新品上市" class="home__link--3" />
        </div>
      </div>
    </div>
    <BannerItem
      v-for="banner in banners"
      :key="banner.index"
      :imgSrc="banner.imgSrc"
      :titleSrc="banner.titleSrc"
      :contents="banner.contents"
      :reverse="banner.reverse"
    />
    <div class="py-1 flex-center">
      <img src="@/assets/img/lg-想吃甜點是不需要理由的.png" alt="">
    </div>
  </div>
</template>

<script>
import LinkItem from '@/components/LinkItem.vue'
import BannerItem from '@/components/BannerItem.vue'
import imgSrc from '@/assets/img/lg-為什麼選擇了做甜點.png'

export default {
  name: 'HomeView',
  components: {
    LinkItem,
    BannerItem
  },
  data () {
    return {
      banners: [
        {
          index: 1,
          imgSrc: 'https://bit.ly/2xPn7Eq',
          titleSrc: imgSrc,
          contents: ['青山依舊在，幾度夕陽紅。慣看秋月春風。一壺濁酒喜相逢，浪花淘盡英雄。是非成敗轉頭空，滾滾長江東逝水，白髮漁樵江渚上，古今多少事，都付笑談中。', '是非成敗轉頭空，滾滾長江東逝水，白髮漁樵江渚上，古今多少事，都付笑談中。']
        },
        {
          index: 2,
          imgSrc: 'https://bit.ly/2zzAQS4',
          titleSrc: imgSrc,
          contents: ['青山依舊在，幾度夕陽紅。慣看秋月春風。一壺濁酒喜相逢，浪花淘盡英雄。是非成敗轉頭空，滾滾長江東逝水，白髮漁樵江渚上，古今多少事，都付笑談中。', '是非成敗轉頭空，滾滾長江東逝水，白髮漁樵江渚上，古今多少事，都付笑談中。'],
          reverse: 'reverse'
        }
      ]
    }
  }
}
</script>
