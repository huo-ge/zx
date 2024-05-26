<script setup lang="ts">
import {reqLogin} from "@/api/user/index"
import { onMounted } from 'vue';

onMounted(() => {
  reqLogin({
    username: 'admin',
    password: '111111'
  }).then(res => {
    console.log(res);
    
  })
})
</script>

<template>
  <div>App</div>
  <div>测试commit- msg</div>
</template>

<style scoped></style>
