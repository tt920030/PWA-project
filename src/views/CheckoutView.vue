<template>
  <div class="row justify-content-center mt-2 mb-5">
    <div class="col-6">
      <div class="check bg-secondary">
        <div class="mb-2">
          <h1>運送</h1>
        </div>
        <div class="row check__row">
          <div class="col-6 check__col">
            <label for="">
              <h3 class="check__label">姓氏</h3>
              <input type="text">
            </label>
          </div>
          <div class="col-6 check__col">
            <label for="">
              <h3 class="check__label">名字</h3>
              <input type="text">
            </label>
          </div>
        </div>
        <div class="row check__row">
          <div class="col-12 check__col">
            <label for="">
              <h3 class="check__label">電話</h3>
              <input type="text">
            </label>
          </div>
        </div>
        <div class="row check__row check__row--input-group align-items-end">
          <div class="col-6 check__col">
            <label for="">
              <h3 class="check__label">地址</h3>
              <input type="text">
            </label>
          </div>
          <div class="col-6 check__col">
            <label for="">
              <input type="text">
            </label>
          </div>
        </div>
        <div class="row check__row">
          <div class="col-12 check__col">
            <label for="">
              <input type="text">
            </label>
          </div>
        </div>
      </div>
      <button class="btn-lg bg-tertiary">
        <h2>下一步</h2>
      </button>
    </div>
    <div class="col-4">
      <div class="order-sum">
        <h2 class="order-sum__title order-sum__title--secondary text-center bg-primary">訂單摘要</h2>
        <div class="order-sum__lines order-sum__lines--secondary">
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
      </div>
    </div>
  </div>
</template>
