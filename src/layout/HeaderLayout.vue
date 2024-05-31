<template>
  <nav class="navbar flex-space-between">
    <div class="navbar__logo-container">
      <img class="navbar__logo" src="@/img/logo-all-dark.svg"/>
    </div>
    <div class="navbar__links flex-center">
      <router-link class="navbar__link" to="/">首頁</router-link>
      <router-link class="navbar__link" to="/product">甜點</router-link>
      <router-link class="navbar__link" to="/login">登入</router-link>
      <router-link class="navbar__link navbar__link--cart" to="/cart">
        <img class="navbar__cart-icon" src="@/img/shopping_cart_24dp.svg"/>
      </router-link>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'HeaderLayout'
}
</script>
