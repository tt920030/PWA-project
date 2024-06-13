<template>
  <div class="login mt-2 mb-5 flex-center">
    <div class="sign bg-secondary">
      <div class="px-2">
        <h1 class="text-center sign__title">會員登入</h1>
        <div class="input-group sign__input-group">
          <span class="material-icons input-group__icon bg-primary">
            person
          </span>
          <input class="input-group__input" type="text" placeholder="電子信箱/手機號碼">
        </div>
        <div class="input-group sign__input-group">
          <span class="material-icons input-group__icon bg-primary">
            vpn_key
          </span>
          <input class="input-group__input" type="text" placeholder="請輸入使用者密碼">
        </div>
        <div class="checkbox-group sign__checkbox-group">
          <label for="rememberMe">
            <input class="checkbox-group__input" type="checkbox" id="rememberMe">
            <span>記住我</span>
          </label>
        </div>
      </div>
      <button class="btn-lg bg-tertiary">
        <h2>登入帳號</h2>
      </button>
    </div>
    <div class="media px-2 bg-primary">
      <h2 class="media__title text-center">—— 連結社群帳號 ——</h2>
      <button class="media__btn btn-sm">
        <img src="@/assets/img/ic-facebook.png">
      </button>
      <button class="media__btn btn-sm">
        <img src="@/assets/img/ic-google.png">
      </button>
      <button class="media__btn btn-sm">
        <img src="@/assets/img/ic-yahoo.png">
      </button>
    </div>
  </div>
</template>
