<template>
  <footer class="footer">
    <div class="_container">
      <div class="footer__row">
        <div class="footer__columns">
          <div class="footer-descriptions">
            <p>Политика конфеденциальности</p>
          </div>
          <div class="footer-descriptions">
            <p>© 2020 «Four group»</p>
          </div>
        </div>
        <div class="footer__columns">
          <div class="footer-icons">
            <a href="" class="footer-icons__item"
              ><img src="../assets/vk.svg" alt=""
            /></a>
            <a href="" class="footer-icons__item"
              ><img src="../assets/inst.svg" alt=""
            /></a>
            <a href="" class="footer-icons__item"
              ><img src="../assets/fb.svg" alt=""
            /></a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.footer {
  padding: 3% 0px 0px 0px;
  &__row {
    display: flex;
    justify-content: space-between;
    background: #fdfbf0;
    border-radius: 20px;
    align-items: flex-end;

    @media (max-width: 759+px) {
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
    }
  }

  &__columns {
    padding: 19px 35px;
  }
}

.footer-descriptions {
  p {
    font-family: Open Sans;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 27px;
    text-transform: uppercase;

    color: #414042;
  }
}
.footer-icons {
  &__item {
    padding: 0px 0px 0px 38px;
  }
}
</style>