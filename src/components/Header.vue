<template>
  <div class="header">
    <div class="container">
      <div class="header-box">
        <div class="header-logo">
          <img src="@/assets/logo.svg" alt="">
        </div>
        <div class="header-lang">
          <router-link to="/" class="header-lang__item">UZ</router-link>
          <router-link to="/" class="header-lang__item">РУ</router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .header{
    padding-top: 25px;
    &-box{
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    &-lang{
      display: flex;
      gap: 13px;
      &__item{
        font-size: 24px;
        font-weight: 700;
        color: #fff;
      }
    }
  }
</style>