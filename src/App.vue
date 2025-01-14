<template>

 <Suspense>
    <template #default>
        <SyncYc></SyncYc>
    </template>
    <template #fallback>
        <div>哈哈哈哈哈哈</div>
    </template>
 </Suspense>>

</template>

<script setup lang='ts'>

import { ref,reactive, defineAsyncComponent } from 'vue' ;
const SyncYc = defineAsyncComponent(()=>import('./SyncComp/SyncYc.vue'))

</script>

<style scoped>

</style>