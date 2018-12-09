<template>
    <el-container>
        <el-header class="header" height="100px">
            <div class="header-wrap">
                <div class="header-logo">
                    <img class="logo" src="../assets/image/logo.jpg">
                    <img class="name" src="../assets/image/name.png">
                </div>
                <div class="header-drop">
                    <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect" style="height: 100%">
                        <el-menu-item index="1">首页</el-menu-item>
                        <el-menu-item index="2">产品展示</el-menu-item>
                        <el-menu-item index="3">新闻资讯</el-menu-item>
                        <el-menu-item index="4">关于我们</el-menu-item>
                    </el-menu>
                </div>
            </div>
        </el-header>
        <el-main>
            <div class="main-banner">
                <el-carousel trigger="click" height="600px">
                    <el-carousel-item v-for="item in 4" :key="item" style="background-color: orange">
                        <h3>{{ item }}</h3>
                    </el-carousel-item>
                </el-carousel>
            </div>
            <div class="main-image">
                <ul>
                    <li>

                    </li>
                </ul>
            </div>
        </el-main>
        <el-footer>Footer</el-footer>
    </el-container>
</template>

<script>
	export default {
		name: "index",
        data(){
		    return {
                activeIndex: '1',


            }
        },
        methods: {

        }
	}
</script>

<style scoped>

</style>
