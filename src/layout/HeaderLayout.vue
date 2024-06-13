<template>
  <header class="container py-2">
    <div class="flex-space-between">
      <img src="@/assets/img/logo-all-dark.png"/>
      <nav class="nav flex-center">
        <router-link class="mr-4" to="/">首頁</router-link>
        <router-link class="mr-4" to="/product">甜點</router-link>
        <router-link class="mr-4" to="/login">登入</router-link>
        <router-link class="nav__icon" to="/cart">
          <span class="material-icons">
            shopping_cart
          </span>
        </router-link>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderLayout'
}
</script>
