<template>

 <Layout></Layout>

</template>

<script setup lang='ts'>

import { ref,reactive } from 'vue' ;
import Layout from './Layout/index.vue';

</script>

<style lang="scss">
#app {
  @include bfc;
}
</style>