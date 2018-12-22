<template>
    <el-container>
        <el-header class="header" height="60px">
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
                        <el-menu-item index="1">首</el-menu-item>
                        <el-menu-item index="2">产品展示</el-menu-item>
                        <el-menu-item index="3">新闻资讯</el-menu-item>
                        <el-menu-item index="4">关于我们</el-menu-item>
                    </el-menu>
                </div>
            </div>
        </el-header>
        <el-main>
            <div class="main-banner">
                <el-carousel
                    trigger="click"
                    height="600px"
                    interval="5000"
                >
                    <el-carousel-item v-for="item in 3" :key="item" :class="'banner'+item" style="background-color: orange">
                        <div>

                        </div>
                    </el-carousel-item>
                </el-carousel>
            </div>
            <div class="main-image">
                <div class="main-title">
                    <h1>产品展示</h1>
                    <div class="main-line"></div>
                </div>
                <div class="show-wrap">
                    <div
                        v-for="(item, i) in showList"
                        :key="i"
                        :class="['show-list','show'+(i+1)]"
                    ></div>
                </div>
            </div>
            <div class="main-me">
                <div class="me-container">
                    <div class="left">
                        <div class="main-title">
                            <h1>新闻动态</h1>
                            <div class="main-line"></div>
                        </div>
                        <div>
                            <img src="@/assets/image/new-img.jpg" alt="">
                            <ul>
                                <li>

                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="right">
                        <div class="main-title">
                            <h1>公司简介</h1>
                            <div class="main-line"></div>
                        </div>

                    </div>

                </div>
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
                showList: [
                    {
                        'background-image': 'url("../../assets/image/s1.png")'
                    },
                    {},
                    {},
                    {}
                ]

            }
        },
        methods: {

        }
	}
</script>

<style scoped>

</style>
