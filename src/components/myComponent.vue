<template>
  <div class="">
    <ul>
      <li
        class="number"
        @click="handleClick"
        :class="{ active: activeNum == 'One' }"
      >
        One
      </li>
      <li class="number">Two</li>
      <li class="number">Three</li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from "vue";

const activeNum = ref(null);

const handleClick = (event) => {
  if (activeNum.value == event.target.innerText) {
    activeNum.value = null;
  } else {
    activeNum.value = event.target.innerText;
  }
};
</script>

<style scoped>
.number {
  cursor: pointer;
  user-select: none;
}
.active {
  color: blue;
}
</style>

