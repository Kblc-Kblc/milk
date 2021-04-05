<template>
  <section class="content">
    <div class="_container">
      <div class="content__row">
        <div class="content__columns">
          <div class="content-body">
            <div class="content-body__new">
              <img :src="image.NewItem" alt="" />
            </div>
            <div class="content-body__item">
              <img :src="image.SubImage" alt="" />
              <img :src="image.SubImageTwo" alt="" />
            </div>
          </div>
        </div>
        <div class="content__columns">
          <div class="content-body">
            <div class="content-body__item">
              <img :src="image.new" alt="" />
              <img :src="image.open" alt="" />
            </div>
            <div class="content-body__new">
              <img :src="image.BlackFriday" alt="" />
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
        NewItem: require("../assets/big-l.jpg"),
        SubImage: require("../assets/little-l.jpg"),
        SubImageTwo: require("../assets/lttle-l.jpg"),

        BlackFriday: require("../assets/01.jpg"),
        open: require("../assets/02.jpg"),
        new: require("../assets/03.jpg"),
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.content {
  padding: 40px 0px 0px 0px;
  &__row {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    margin: 0px -10px;

    @media (max-width: 1452+px) {
      flex-direction: column;
      align-items: center;
    }
  }

  &__columns {
    flex: 1 1 50%;
    padding: 0px 10px;
  }
}

.content-body {
  &__new {
    img {
      margin: 0px 0px 15px 0px;
      width: 709px;
      height: 470px;
      border-radius: 15px;
      object-fit: cover;

      @media (max-width: 767.98+px) {
        width: 310px;
        height: 260px;
      }
    }
  }

  &__item {
    display: flex;
    justify-content: space-between;

    @media (max-width: 767.98+px) {
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
    img {
      margin: 0px 0px 17.5px 0px;

      width: 344px;
      height: 232px;
      border-radius: 15px;
      object-fit: cover;

      @media (max-width: 767.98+px) {
        width: 310px;
        height: 260px;
      }
    }
  }
}
</style>