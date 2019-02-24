<template>
    <div class="xt-header" height="60px">
        <div class="header-wrap">
            <div class="header-logo">
                <img class="logo" src="../assets/image/yer-logo1.png">
            </div>
            <div class="header-drop">
                <el-menu
                    :default-active="activeIndex"
                    class="el-menu-demo"
                    mode="horizontal"
                    background-color="#545c64"
                    text-color="#fff"
                    active-text-color="#ffd04b"
                    @select="handleSelect"
                    style="height: 100%"
                >
                    <el-menu-item index="1">首页</el-menu-item>
                    <el-menu-item index="2">产品展示</el-menu-item>
                    <el-menu-item index="3">新闻资讯</el-menu-item>
                    <el-menu-item index="4">关于我们</el-menu-item>
                </el-menu>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "header",
        data(){
            return {
                activeIndex: '1',


            }
        },
    }
</script>

<style scoped>

</style>
