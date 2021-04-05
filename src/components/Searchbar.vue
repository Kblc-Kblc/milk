<template>
  <div class="searchbar">
    <div class="_container">
      <div class="searchbar__row">
        <div class="searchbar__columns">
          <div class="searchbar-section">
            <div class="searchbar-section__logo">
              <router-link to="/" active-class="active">
                <img src="../assets/logo.png" alt="" />
              </router-link>
            </div>
          </div>
        </div>
        <div class="searchbar__columns">
          <div class="searchbar-section">
            <div class="searchbar-section__catalog">
              <div class="hamburger-menu">
                <div class="searchbar-section__subtitle"><p>Каталог</p></div>
                <input id="menu__toggle" type="checkbox" />
                <label class="menu__btn" for="menu__toggle">
                  <span></span>
                </label>

                <ul class="menu__box">
                  <router-link
                    tag="li"
                    to="/kitchen"
                    exact
                    active-class="active"
                    ><a class="menu__item" href="#"
                      >Акции и скидки</a
                    ></router-link
                  >
                  <router-link tag="li" to="/kitchen" active-class="active"
                    ><a class="menu__item" href="#">Кухни</a></router-link
                  >
                  <router-link tag="li" to="/kitchen" active-class="active"
                    ><a class="menu__item" href="#">Детские</a></router-link
                  >
                  <router-link tag="li" to="/kitchen" active-class="active"
                    ><a class="menu__item" href="#">Спальни</a></router-link
                  >
                  <router-link tag="li" to="/kitchen" active-class="active"
                    ><a class="menu__item" href="#"
                      >Корпусная мебель</a
                    ></router-link
                  >
                  <router-link tag="li" to="/kitchen" active-class="active"
                    ><a class="menu__item" href="#"
                      >Офисная мебель</a
                    ></router-link
                  >
                  <router-link tag="li" to="/kitchen" active-class="active">
                    <a class="menu__item" href="#">Торговое оборудование</a>
                  </router-link>
                  <router-link tag="li" to="/kitchen" active-class="active"
                    ><a class="menu__item" href="#">Услуги</a></router-link
                  >
                  <router-link tag="li" to="/kitchen" active-class="active"
                    ><a class="menu__item" href="#">Статьи</a></router-link
                  >
                </ul>
              </div>
            </div>
          </div>
        </div>
        <div class="searchbar__columns">
          <div class="searchbar-section">
            <div class="searchbar-section__search">
              <input
                autocomplete="off"
                type="text"
                class="searchbar-section__input"
              />
            </div>
          </div>
        </div>
        <div class="searchbar-info-flex">
          <div class="searchbar__columns">
            <div class="searchbar-section">
              <div class="searchbar-section__payment">
                <img src="../assets/pay.png" alt="" />
              </div>
              <div class="searchbar-section__subtitle">
                <a href="#">Оплата</a>
              </div>
            </div>
          </div>
          <div class="searchbar__columns">
            <div class="searchbar-section">
              <div class="searchbar-section__payment">
                <img src="../assets/drive.png" alt="" />
              </div>
              <div class="searchbar-section__subtitle">
                <a href="#">Доставка</a>
              </div>
            </div>
          </div>
          <div class="searchbar__columns">
            <div class="searchbar-section">
              <div class="searchbar-section__payment">
                <img src="../assets/like.png" alt="" />
              </div>
              <div class="searchbar-section__subtitle">
                <a href="#">Лайк</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.searchbar {
  padding: 10px 0px 0px 0px;
  &__row {
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    flex-wrap: wrap;
    @media (max-width: 1452+px) {
      flex-direction: column;
      align-items: center;
    }
  }

  &__columns {
  }
}

.searchbar-section {
  &__logo {
    margin: -40px 0px 0px 0px;
    @media (max-width: 1452+px) {
      margin: 0px 0px;
      padding: 0px 0px 30px 0px;
    }
  }

  &__catalog {
    text-align: center;
    background: #ffffff;
    border: 2px solid rgba(0, 0, 0, 0.1);
    border-radius: 10px;
    padding: 12px 25px 0px 70px;

    position: relative;
    @media (max-width: 1452+px) {
      margin: 0px 0px 30px 0px;
    }
  }

  &__subtitle {
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 20px;

    text-transform: uppercase;

    color: #494949;
  }

  &__search {
    width: 610px;
    height: 51px;
    position: relative;
    @media (max-width: 1452+px) {
      margin: 0px 0px 30px 0px;
    }
    @media (max-width: 767.98+px) {
      width: 310px;
    }

    &:before {
      content: "";
      position: absolute;
      top: 0;
      bottom: 0;
      right: 3%;
      margin: auto 0;
      width: 25px;
      height: 25px;
      background: url("../assets/sear.svg") right no-repeat;
      background-size: cover;
    }
  }

  &__input {
    width: 100%;
    height: 100%;
    background: #ffffff;
    border: 2px solid rgba(0, 0, 0, 0.1);
    border-radius: 10px;
    padding: 0px 15px;
    &:focus {
      border: 2px solid #c9d6a4;
    }
  }

  &__payment {
    text-align: center;

    img {
      height: 47px;
      padding: 0px 0px 10px 0px;
    }
  }

  &__subtitle {
    text-align: center;
    a {
      font-style: normal;
      font-weight: normal;
      font-size: 20px;
      color: #494949;
    }
  }
}
.searchbar-info-flex {
  display: flex;
  gap: 20px;
}
//<бургер>===============================================================================================
#menu__toggle {
  opacity: 0;
}

#menu__toggle:checked ~ .menu__btn > span {
  transform: rotate(45deg);
}
#menu__toggle:checked ~ .menu__btn > span::before {
  top: 0;
  transform: rotate(0);
}
#menu__toggle:checked ~ .menu__btn > span::after {
  top: 0;
  transform: rotate(90deg);
}
#menu__toggle:checked ~ .menu__box {
  visibility: visible;
  left: 0;
}

.menu__btn {
  display: flex;
  align-items: center;
  position: absolute;
  top: 20%;
  left: 10%;

  width: 26px;
  height: 26px;

  cursor: pointer;
  z-index: 1;
}

.menu__btn > span,
.menu__btn > span::before,
.menu__btn > span::after {
  display: block;
  position: absolute;

  width: 100%;
  height: 2px;

  background-color: #616161;

  transition-duration: 0.25s;
}
.menu__btn > span::before {
  content: "";
  top: -8px;
}
.menu__btn > span::after {
  content: "";
  top: 8px;
}

.menu__box {
  display: block;
  position: fixed;
  visibility: hidden;
  z-index: 99;
  top: 0;
  left: -100%;

  width: 300px;
  height: 100%;

  margin: 0;
  padding: 80px 0;

  list-style: none;

  background-color: #c9d6a4;
  box-shadow: 1px 0px 6px rgba(0, 0, 0, 0.2);

  transition-duration: 0.25s;
}

.menu__item {
  display: block;
  padding: 12px 24px;

  color: #333;

  font-family: "Roboto", sans-serif;
  font-size: 20px;
  font-weight: 600;

  text-decoration: none;

  transition-duration: 0.25s;
}
.menu__item:hover {
  background-color: #cfd8dc;
}
//</бургер>===============================================================================================
</style>