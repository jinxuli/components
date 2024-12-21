<template>
    <div>
        <div>
            <span class="box">sdfsfsdf</span>
        </div>
        {{ state }}
        <el-button @click="changeName">点击</el-button>
        {{ test }}
    </div>
</template>
<script setup>
import test from '@assets/vue.svg';
defineOptions({
    name: 'XFlow',
});

const state = ref('');

const changeName = (a, b) => {
    state.value = 'XFlow updated';
};
onMounted(() => {
    console.log('');
    console.log('sdffdssd');
});
</script>
<style scoped lang="less">
.box {
    background-color: @primary;
}
</style>
