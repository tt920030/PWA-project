<template>
  <nav class="navbar container py-2">
    <div class="flex-space-between">
      <img src="@/assets/img/logo-all-dark.png"/>
      <div class="flex-center">
        <router-link class="mr-4" to="/">首頁</router-link>
        <router-link class="mr-4" to="/product">甜點</router-link>
        <router-link class="mr-4" to="/login">登入</router-link>
        <router-link class="navbar__icon" to="/cart">
          <span class="material-icons">
            shopping_cart
          </span>
        </router-link>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'HeaderLayout'
}
</script>
