<template>
  <div class="top">
    <div class="top__left">
      <img src="@/assets/images/location.svg" alt="location">
      <span>Москва</span>
    </div>
    <div class="top__right">
      <ul class="top__list">
        <li v-for="(item, i) in nav" :key="`nav__${i}`">
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup lang="ts">
const nav = [
  "Бренды", "Доставка", "Возврат", "Документация", "Контакты"
]
</script>

<style scoped lang="scss">
.top {
  padding: 0.5rem 10rem;
  background-color: #F6F6F6;

  display: flex;
  justify-content: space-between;
  align-items: center;

  &__left {
    display: flex;
    gap: 0.5rem;
    align-items: center;
  }

  &__list {
    display: flex;
    gap: 1rem;
  }
}
</style>