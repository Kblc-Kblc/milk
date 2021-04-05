<template>
  <header class="navbar">
    <div class="_container">
      <div class="navbar__row">
        <div class="navbar__coumns">
          <div class="navbar-section">
            <a
              href="mailto: mebel@mail.ru"
              class="navbar-section__mail _icon-mail"
              >mebel@mail.ru</a
            >
          </div>
        </div>
        <div class="navbar__coumns">
          <div class="navbar-section">
            <a href="#" class="navbar-section__adress _icon-loc"
              >Санкт-Петербург, ул. Ленина, д. 1</a
            >
          </div>
        </div>
        <div class="navbar__coumns">
          <div class="navbar-section">
            <a href="tel: +79119859822" class="navbar-section__phone _icon-tel"
              >+ 7 911 985 98 22</a
            >
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.navbar {
  padding: 10px 0px;
  background-color: #c9d6a4;
  &__row {
    display: flex;
    justify-content: flex-end;

    @media (max-width: 1452+px) {
      justify-content: space-between;
    }

    @media (max-width: 991+px) {
      flex-direction: column;
    }
  }

  &__coumns {
    padding: 0px 0px 0px 30px;
  }
}

.navbar-section {
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 35px;
  @media (max-width: 404+px) {
    max-width: 200px;
  }
  &__mail {
    color: rgba(27, 32, 6, 0.8);
    &::before {
      padding: 0px 13px 0px 0px;
    }
  }

  &__adress {
    color: rgba(27, 32, 6, 0.8);
    &::before {
      padding: 0px 13px 0px 0px;
    }
  }

  &__phone {
    color: rgba(27, 32, 6, 0.8);
    &::before {
      padding: 0px 13px 0px 0px;
    }
  }
}
</style>