<template>
  <section class="room">
    <div class="_container">
      <div class="room__title"><h2>Комнаты</h2></div>
      <div class="room__row">
        <div class="room__columns">
          <div class="room-body">
            <div class="room-body__columns">
              <div class="room-body__image">
                <img class="room-body__sofa" :src="image.sofa" alt="" />
              </div>
              <div class="room-body__image">
                <img class="room-body__cantry" :src="image.SofaCantry" alt="" />
              </div>
            </div>
            <div class="room-body__columns">
              <div class="room-body__image">
                <img class="room-body__vintage" :src="image.vintage" alt="" />
              </div>
              <div class="room-body__image">
                <img class="room-body__yellow" :src="image.yellow" alt="" />
              </div>
            </div>
          </div>
        </div>
        <div class="room__columns">
          <div class="room-body">
            <div class="room-body__columns">
              <div class="room-body__image">
                <img class="room-body__sofa" :src="image.TestOne" alt="" />
              </div>
              <div class="room-body__image">
                <img class="room-body__cantry" :src="image.TestTwo" alt="" />
              </div>
            </div>
            <div class="room-body__columns">
              <div class="room-body__image">
                <img class="room-body__vintage" :src="image.TestTwo" alt="" />
              </div>
              <div class="room-body__image">
                <img class="room-body__yellow" :src="image.TestOne" alt="" />
              </div>
            </div>
          </div>
        </div>
        <div class="room__columns">
          <div class="room-body">
            <div class="room-body__columns">
              <div class="room-body__image">
                <img class="room-body__sofa" :src="image.sofa" alt="" />
              </div>
              <div class="room-body__image">
                <img class="room-body__cantry" :src="image.SofaCantry" alt="" />
              </div>
            </div>
            <div class="room-body__columns">
              <div class="room-body__image">
                <img class="room-body__vintage" :src="image.vintage" alt="" />
              </div>
              <div class="room-body__image">
                <img class="room-body__yellow" :src="image.yellow" alt="" />
              </div>
            </div>
          </div>
        </div>
        <div class="room__columns">
          <div class="room-body">
            <div class="room-body__columns">
              <div class="room-body__image">
                <img class="room-body__sofa" :src="image.sofa" alt="" />
              </div>
              <div class="room-body__image">
                <img class="room-body__cantry" :src="image.SofaCantry" alt="" />
              </div>
            </div>
            <div class="room-body__columns">
              <div class="room-body__image">
                <img class="room-body__vintage" :src="image.vintage" alt="" />
              </div>
              <div class="room-body__image">
                <img class="room-body__yellow" :src="image.yellow" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      image: {
        sofa: require("../assets/room-one.jpg"),
        SofaCantry: require("../assets/room-three.jpg"),
        vintage: require("../assets/room-two.jpg"),
        yellow: require("../assets/room-four.png"),

        TestOne: require("../assets/itemhi.jpg"),
        TestTwo: require("../assets/item.jpg"),
        TestThree: require("../assets/bad.jpg"),
      },
    };
  },
};
</script>

<style  lang="scss" scoped>
.room {
  padding: 100px 0px 0px 0px;
  &__row {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    @media (max-width: 1452+px) {
      flex-direction: column;
      align-items: center;
    }
  }

  &__columns {
  }

  &__title {
    font-style: normal;
    font-weight: normal;
    font-size: 35px;
    line-height: 50px;

    text-transform: uppercase;
    color: #494949;

    padding: 0px 0px 40px 0px;

    @media (max-width: 1452+px) {
      text-align: center;
    }
  }
}

.room-body {
  display: flex;
  flex-wrap: wrap;
  margin: 0px -10px;

  @media (max-width: 732+px) {
    justify-content: center;
    align-items: center;
  }

  &__columns {
    padding: 0px 10px;
  }

  &__image {
    text-align: right;
    padding: 0px 0px 30px 0px;
  }

  &__sofa {
    width: 344px;
    height: 507px;
    object-fit: cover;
  }

  &__cantry {
    width: 344px;
    height: 306px;
    object-fit: cover;
  }

  &__vintage {
    width: 345px;
    height: 306px;
    object-fit: cover;
  }

  &__yellow {
    width: 345px;
    height: 507px;
    object-fit: cover;
  }
}
</style>