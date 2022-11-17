<template>
  <div class="about">
    <h1>This is an Play page</h1>
    <myComponent />
  </div>
</template>

<script setup>
import myComponent from "@/components/myComponent.vue";
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
