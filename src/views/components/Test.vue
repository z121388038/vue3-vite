<template>
  <div class="test">
    <h2>{{ msg }}</h2>
    <p>{{ user.name }}</p>
    <p>{{ user.age }}</p>
    <p>{{ user.area }}</p>
  </div>
</template>

<script setup lang="ts">
import { reactive, ref } from 'vue';

const msg = ref('消息提示');
const user = reactive({
  name: '张三',
  age: 24,
  area: '上海',
});
</script>

<style scoped lang="scss"></style>
