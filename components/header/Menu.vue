<template>
<div class="title">
    <el-menu
        :default-active="activeIndex2"
        class="el-menu-demo"
        mode="vertical"
        router
        @select="handleSelect"
        background-color="#545c64"
        text-color="#fff"
        active-text-color="#ffd04b">
        <el-menu-item index="/">demo1</el-menu-item>
        <el-menu-item index="/firstDemo">demo2</el-menu-item>
        <el-menu-item index="3">demo3</el-menu-item>
        <el-menu-item index="4">demo4</el-menu-item>
        <el-menu-item index="5">demo5</el-menu-item>
    </el-menu>
</div>
</template>

<script>
export default {
    data() {
        return {
            activeIndex2: '1'
        }
    },
    methods: {
        handleSelect(key, keyPath){
            console.log(key);
        }
    }
}
</script>

<style>
.title {
    width: 300px;
}
.title ul {
    height: calc(100vh - 52px);
}
</style>