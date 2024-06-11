<template>
  <footer class="footer">
    <div class="container bg-secondary py-2">
      <div class="row justify-content-center">
        <div class="col-10 flex-space-between">
          <div class="flex-center">
            <img
              class="footer__logo-icon"
              src="@/assets/img/logo-light.png"
            >
            <h2>訂閱你我的甜蜜郵件</h2>
          </div>
          <div class="sendMail input-container d-flex">
            <div class="p-relative w-100">
              <span class="sendMail__input-icon p-absolute material-icons">
                email
              </span>
              <input
                class="sendMail__input w-100 h-100 bg-primary"
                type="text"
              >
            </div>
            <button class="sendMail__btn bg-tertiary">
              <span class="material-icons">
                arrow_forward
              </span>
            </button>
          </div>
        </div>
      </div>
    </div>
    <div class="container bg-primary py-2">
      <div class="row justify-content-center">
        <div class="col-10 flex-space-between">
          <div>
            <img
              class="footer__logo-text"
              src="@/assets/img/logotype-lg-dark.png"
            >
            <p class="footer__info">07-1234-5678</p>
            <p class="footer__info">sweetaste@email.com</p>
            <p class="footer__info mb-2">
              800 高雄市新興區幸福路 520 號
            </p>
            <div>
              <img
                class="footer__icon-media"
                src="@/assets/img/ic-line@.svg"
              >
              <img
                class="footer__icon-media"
                src="@/assets/img/ic-facebook.svg"
              >
            </div>
          </div>
          <div class="flex-space-between flex-column align-items-end h-100">
            <img src="@/assets/img/sm-今天是個吃甜點的好日子.png">
            <p class="footer__copyRight">
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
