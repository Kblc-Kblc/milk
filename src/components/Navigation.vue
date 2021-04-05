<template>
  <nav class="navigatons">
    <div class="_container">
      <ul class="navigatons-list">
        <router-link tag="li" to="/kitchen" exact active-class="active">
          <a class="navigatons-list__item" href="#">Акции и скидки</a>
        </router-link>
        <router-link tag="li" to="/kitchen" active-class="active">
          <a class="navigatons-list__item" href="#">Кухни</a>
        </router-link>
        <router-link tag="li" to="/kitchen" active-class="active">
          <a class="navigatons-list__item" href="#">Детские</a>
        </router-link>
        <router-link tag="li" to="/kitchen" active-class="active">
          <a class="navigatons-list__item" href="#">Спальни</a>
        </router-link>
        <router-link tag="li" to="/kitchen" active-class="active">
          <a class="navigatons-list__item" href="#">Корпусная мебель</a>
        </router-link>
        <router-link tag="li" to="/kitchen" active-class="active">
          <a class="navigatons-list__item" href="#">Офисная мебель</a>
        </router-link>
        <router-link tag="li" to="/kitchen" active-class="active">
          <a class="navigatons-list__item" href="#">Торговое оборудование</a>
        </router-link>
        <router-link tag="li" to="/kitchen" active-class="active">
          <a class="navigatons-list__item" href="#">Услуги</a>
        </router-link>
        <router-link tag="li" to="/kitchen" active-class="active">
          <a class="navigatons-list__item" href="#">Статьи</a>
        </router-link>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.navigatons {
  @media (max-width: 1452+px) {
    display: none;
  }
  padding: 36px 0px 0px 0px;
}

.navigatons-list {
  display: flex;
  justify-content: space-between;
  &__item {
    display: inline-block;
    font-family: Open Sans;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 40px;

    text-transform: uppercase;

    color: #494949;

    display: inline-block;
    position: relative;
    &:after {
      background: none repeat scroll 0 0 transparent;
      bottom: 0;
      content: "";
      display: block;
      height: 2px;
      left: 50%;
      position: absolute;
      background: #494949;
      transition: width 0.3s ease 0s, left 0.3s ease 0s;
      width: 0;
    }
    &:hover:after {
      width: 100%;
      left: 0;
    }
  }
}
</style>