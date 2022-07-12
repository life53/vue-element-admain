<template>
    <div id="app">
        <!-- <router-view /> -->
    </div>
</template>
<script>
// 引入接口
import { getListAPI } from "@/api";
export default {
    created() {
        this.getListFn();
    },
    // 请求方法并请求数据
    methods: {
        async getListFn() {
            const res = await getListAPI();
            console.log(res);
        },
    },
};
</script>

<style>
</style>
