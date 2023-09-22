<template>
  <header>
    <HeaderTop />
    <div class="header">
      <img class="header__logo" src="@/assets/images/logo.png" alt="logo">
      <button class="header__catalog">
        <img src="@/assets/images/catalog.svg" alt="catalog">
        <span>Каталог</span>
      </button>
      <input class="header__search" type="text" placeholder="Поиск">
      <div class="header__account">
        <div class="header__profile">
          <img src="@/assets/images/profile.svg" alt="profile">
          <span>Профиль</span>
        </div>
        <div class="header__orders">
          <img src="@/assets/images/orders.svg" alt="Заказы">
          <span>Заказы</span>
        </div>
        <div class="header__cart">
          <img src="@/assets/images/cart.svg" alt="Корзина">
          <span>Корзина</span>
        </div>
      </div>
    </div>
    <HeaderBottom />
  </header>
</template>

<script setup lang="ts">

</script>

<style scoped lang="scss">
.header {
  padding: 1rem 10rem;
  display: grid;
  grid-template-columns: 2fr 1fr 10fr 2fr;
  align-items: center;
  gap: 1.5rem;

  &__catalog {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    font-weight: 500;
    font-size: 1.125rem;
    background-color: #fcec41;
    padding: 1rem 2rem;
  }

  &__account {
    display: flex;
    align-items: center;
    gap: 1.5rem;
  }

  &__search {
    border-bottom: 1px solid #D1D1D3;
    color: #D1D1D3;
    padding: 1rem;
    font-weight: 500;
    font-size: 1.25rem;
    line-height: 24.48px;

    background-image: url('@/assets/images/search.svg');
    background-position: right 10px center;
    background-repeat: no-repeat;
  }

  &__profile,
  &__orders,
  &__cart {
    display: flex;
    align-items: center;
    flex-direction: column;
  }
}
</style>