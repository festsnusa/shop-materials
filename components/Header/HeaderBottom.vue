<template>
  <div class="bottom">
    <ul class="bottom__list">
      <li class="bottom__item" v-for="(link, i) in links" :key="`links__${i}`">
        {{ link }}
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
const links = [
  "Акции", "Строительные материалы", "Керамическая плитка", "Краски", "Сантехника", "Напольные покрытия", "Инструменты", "Обои", "Окна"
]
</script>

<style scoped lang="scss">
.bottom {
  border-top: 1px solid #E8E9EA;
  padding: 1rem 10rem;

  &__list {
    display: flex;
    justify-content: space-around;
  }
}
</style>