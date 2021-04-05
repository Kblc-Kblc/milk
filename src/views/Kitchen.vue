<template>
  <div>
    <NavBar />
    <Searchbar />
    <Navigation />
    <div class="kitchen">
      <div class="_container">
        <Breadcrumbs />
        <div class="kitchen__row">
          <div class="kitchen__columns">
            <div class="kitchen__left-top">
              <div class="kitchen-info">
                <div class="kitchen-info__title"><h3>Классика 1</h3></div>
                <div class="kitchen-info__price">
                  <p>80 000 <span>Ꝑ</span></p>
                </div>
                <div class="kitchen-info__articul"><p>Артикул: 405268</p></div>
              </div>
              <div class="kitchen-credits">
                <div class="kitchen-credits__link">
                  <a href="#">Купить в рассрочку</a>
                </div>
                <div class="kitchen-credits__description">
                  <p>от 3000 и в месяц</p>
                </div>
              </div>
              <div class="kitchen__hl"></div>
              <div class="kitchen-promotions">
                <div class="kitchen-promotions__delivery">
                  <p>Бесплатная доставка от 10 000 Ꝑ</p>
                </div>
                <div class="kitchen-promotions__availability">
                  <p>Проверить наличие</p>
                </div>
                <div class="kitchen-promotions__dimensions">
                  <p>Габариты: 160x200x80 см</p>
                </div>
                <div class="kitchen-promotions__weight">
                  <p>Вес: 45 кг</p>
                </div>
              </div>
            </div>
            <div class="kitchen__left-bottom">
              <p>
                Эта кровать классического дизайна будет прекрасно смотреться с
                вашей мебелью и текстилем для спальни. Легко создать гармоничный
                интерьер можно, дополнив другими товарами.
              </p>
              <p>
                Два больших ящика превращают пустующее пространство под кроватью
                в практичное решение для хранения одеял, подушек и постельного
                белья. В комбинацию входят узкий и широкий ящик, что позволяет
                организовать удобно хранение, разделив одеяла и постельное
                белье.
              </p>
            </div>
          </div>
          <div class="kitchen__columns">
            <div class="kitchen__right-top">
              <div class="kitchen__image">
                <img class="kitchen__big" :src="image.KitchenBig" alt="" />
              </div>
              <div class="kitchen__image-three">
                <img class="kitchen__sub" :src="image.KitchenOne" alt="" />
                <img class="kitchen__sub" :src="image.KitchenTwo" alt="" />
                <img class="kitchen__sub" :src="image.KitchenThree" alt="" />
              </div>
            </div>
            <div class="kitchen__right-bottom">
              <p>
                Эта кровать классического дизайна будет прекрасно смотреться с
                вашей мебелью и текстилем для спальни. Легко создать гармоничный
                интерьер можно, дополнив другими товарами.
              </p>
              <p>
                Два больших ящика превращают пустующее пространство под кроватью
                в практичное решение для хранения одеял, подушек и постельного
                белья. В комбинацию входят узкий и широкий ящик, что позволяет
                организовать удобно хранение, разделив одеяла и постельное
                белье.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Breadcrumbs from "@/components/Breadcrumbs";
import NavBar from "@/components/Navbar";
import Searchbar from "@/components/Searchbar";
import Navigation from "@/components/Navigation";
import Footer from "@/components/Footer";

export default {
  data() {
    return {
      image: {
        KitchenBig: require("../assets/k-big.jpg"),
        KitchenOne: require("../assets/k-left.jpg"),
        KitchenTwo: require("../assets/k-middle.jpg"),
        KitchenThree: require("../assets/k-right.jpg"),
      },
    };
  },
  components: {
    Breadcrumbs,
    NavBar,
    Searchbar,
    Navigation,
    Footer,
  },
};
</script>

<style lang="scss" scoped>
.kitchen {
  padding: 22px 0px 0px 0px;
  &__row {
    padding: 10px 0px 0px 0px;
    display: flex;
    justify-content: space-between;

    @media (max-width: 1452+px) {
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    margin: 0px -10px;
  }

  &__columns {
    flex: 1 1 auto;
    padding: 0px 10px;
  }

  &__left-top {
    background: #fdfbf0;
    border-radius: 15px;

    padding: 15px 0px 0px 30px;
    margin: 0px 0px 20px 0px;
  }

  &__hl {
    width: 654.76px;
    border: 1px solid #94af4a;

    margin: 0px 0px 40px 0px;

     @media (max-width: 1452+px) {
          width: 310px;

    }
  }

  &__left-bottom {
    background: #fdfbf0;
    border-radius: 15px;
    p {
      font-style: normal;
      font-weight: normal;
      font-size: 16px;
      line-height: 27px;
      color: #000000;

      padding: 15px 35px;
    }
  }

  &__right-top {
  }

  &__image {
    padding: 0px 0px 20px 0px;
    @media (max-width: 1452+px) {
      text-align: center;
      padding: 20px 0px 20px 0px;
    }
  }

  &__image-three {
    display: flex;
    justify-content: space-between;
    padding: 0px 0px 20px 0px;
    @media (max-width: 1452+px) {
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 20px;
    }
  }

  &__right-bottom {
    background: #fdfbf0;
    border-radius: 15px;
    p {
      font-style: normal;
      font-weight: normal;
      font-size: 16px;
      line-height: 27px;
      color: #000000;

      padding: 15px 35px;
    }
  }

  &__big {
    width: 709px;
    height: 355.34px;
    object-fit: cover;

    @media (max-width: 1452+px) {
      width: 310px;
      height: 260px;
    }
  }

  &__sub {
    width: 222.96px;
    height: 150.82px;
    object-fit: cover;

    @media (max-width: 1452+px) {
      width: 310px;
      height: 260px;
    }
  }
}

.kitchen-info {
  padding: 0px 0px 30px 0px;
  &__title {
    font-style: normal;
    font-weight: normal;
    font-size: 40px;
    line-height: 55px;

    text-transform: uppercase;

    color: #494949;
  }

  &__price {
    font-style: normal;
    font-weight: 700;
    font-size: 40px;
    line-height: 55px;
    text-transform: uppercase;

    color: #494949;
  }

  &__articul {
    font-style: normal;
    font-weight: 700;
    font-size: 14px;
    line-height: 35px;
    text-transform: uppercase;

    color: #494949;
  }
}

.kitchen-credits {
  padding: 0px 0px 26px 0px;
  &__link {
    a {
      font-style: normal;
      font-weight: normal;
      font-size: 17px;
      line-height: 28px;
      text-transform: uppercase;
      color: #708208;
    }
  }

  &__description {
    P {
      font-style: normal;
      font-weight: normal;
      font-size: 17px;
      line-height: 28px;
      text-transform: uppercase;
      color: #000;
    }
  }
}

.kitchen-promotions {
  padding: 0px 0px 35px 0px;
  font-style: normal;
  font-weight: normal;
  font-size: 21px;
  line-height: 30px;
  color: #494949;

  &__delivery {
    position: relative;
    padding: 0px 0px 20px 60px;
    &:before {
      content: "";
      position: absolute;
      left: 0;
      top: 0;
      width: 37px;
      height: 38px;
      background: url("../assets/icon-car.png") left no-repeat;
    }
  }

  &__availability {
    position: relative;
    padding: 0px 0px 20px 60px;

    &:before {
      content: "";
      position: absolute;
      left: 0;
      top: 0;
      width: 36px;
      height: 38px;
      background: url("../assets/geo.png") left no-repeat;
    }
  }

  &__dimensions {
    position: relative;
    padding: 0px 0px 20px 60px;
    &:before {
      content: "";
      position: absolute;
      left: 0;
      top: 0;
      width: 36px;
      height: 38px;
      background: url("../assets/string.png") left no-repeat;
    }
  }

  &__weight {
    position: relative;
    padding: 0px 0px 0px 60px;
    &:before {
      content: "";
      position: absolute;
      left: 0;
      top: 0;
      width: 36px;
      height: 38px;
      background: url("../assets/pak.png") left no-repeat;
    }
  }
}
</style>