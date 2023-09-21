<template>
  <header class="header">
    <div class="header__left">
      <img class="header__logo" src="@/assets/images/logo.png" alt="logo">
    </div>
    <div class="header__right">
      <button class="header__catalog">
        <img src="@/assets/images/catalog.svg" alt="catalog">
        <span>Каталог</span>
      </button>

    </div>

  </header>
</template>

<script setup lang="ts">

</script>

<style scoped lang="scss">
.header {
  padding: 1rem 5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;

  &__catalog {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    font-weight: 500;
    font-size: 1.125rem;
    background-color: #fcec41;
  }
}
</style>