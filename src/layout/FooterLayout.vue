<template>
  <footer class="footer">
    <div class="subscribe container bg-secondary py-2">
      <div class="row justify-content-center">
        <div class="col-10 flex-space-between">
          <div class="flex-center">
            <img
              class="subscribe__logo-icon"
              src="@/assets/img/logo-light.png"
            >
            <h2>訂閱你我的甜蜜郵件</h2>
          </div>
          <div class="subscribe__input-container d-flex">
            <div class="input-group p-relative w-100 bg-primary">
              <span class="input-group__icon p-absolute material-icons">
                email
              </span>
              <input
                class="input-group__input"
                type="text"
              >
            </div>
            <button class="subscribe__btn btn-sm bg-tertiary">
              <span class="material-icons">
                arrow_forward
              </span>
            </button>
          </div>
        </div>
      </div>
    </div>
    <div class="info container bg-primary py-2">
      <div class="row justify-content-center">
        <div class="col-10 flex-space-between">
          <div>
            <img
              class="info__logo"
              src="@/assets/img/logotype-lg-dark.png"
            >
            <p class="info__text">07-1234-5678</p>
            <p class="info__text">sweetaste@email.com</p>
            <p class="info__text mb-2">
              800 高雄市新興區幸福路 520 號
            </p>
            <div>
              <img
                class="info__icon"
                src="@/assets/img/ic-line@.svg"
              >
              <img
                class="info__icon"
                src="@/assets/img/ic-facebook.svg"
              >
            </div>
          </div>
          <div class="flex-space-between flex-column align-items-end h-100">
            <img src="@/assets/img/sm-今天是個吃甜點的好日子.png">
            <p class="info__copyRight">
              © 2018 Sweetaste* All Rights Reserved
            </p>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterLayout'
}
</script>
