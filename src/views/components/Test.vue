<template>
  <div class="test">
    <h2>{{ msg }}</h2>
    <p>{{ user.name }}</p>
    <p>{{ user.age }}</p>
    <p>{{ user.area }}</p>
    <p>{{ filterArr }}</p>
  </div>
</template>

<script setup lang="ts">
import { computed, reactive, ref } from 'vue';

const msg = ref('消息提示');
const user = reactive({
  name: '张三',
  age: 24,
  area: '上海浦东新区',
});

const filterArr = computed(() => [1, 2, 3, 4, 5, 6, 7, 8, 9, 0].filter((item) => item > 5));
</script>

<style scoped lang="scss"></style>
