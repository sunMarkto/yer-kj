<template>
    <div>
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
                        <ul class="new-list">
                            <li>
                                <router-link to="/">
                                    <div class="con">
                                        总结2018，展望2019，感恩所有的伙伴！
                                    </div>
                                    <div class="time">
                                        2019-01-10
                                    </div>
                                </router-link>
                            </li>
                            <li>
                                <router-link to="/">
                                    <div class="con">
                                        关于河北亿尔锐电子科技发展有限公司
                                    </div>
                                    <div class="time">
                                        2018-12-24
                                    </div>
                                </router-link>
                            </li>
                            <li>
                                <router-link to="/">
                                    <div class="con">
                                        亿尔锐官网（www.yerkj.com）
                                    </div>
                                    <div class="time">
                                        2018-12-21
                                    </div>
                                </router-link>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="right">
                    <div class="main-title">
                        <h1>公司简介</h1>
                        <div class="main-line"></div>
                    </div>
                    <p class="companyInfo">
                        河北亿尔锐电子科技有限公司（www.yerkj.com）成立于2013年。公司自成立之初一直专注于大屏商显产品领域，是集大屏商显产品研发、透明屏、安防工程等综合性高科技企业。

                        　　公司非常注重产品质量，以质量赢取口碑一直是公司的经营宗旨。从设计到初稿，从定稿到选材再到安装都谨慎把关，公司都有着非常完善的作业说明以及检测流程;公司都严格要求，一定要做到顾客无可挑剔。正是因为公司从上到下对品质的严格把关，经过五年时间发展，亿尔锐这个品牌才得以在短短的几年内挤身国内同行业一流企业!

                        　　创新是一个民族进步的灵魂!对一个民族尚且如此，何况是一个公司品牌?公司深知这其中的道理，对研发格外重视!公司工程开发部共有8名研发工程师，其中软件工程师2名，硬件工程师3名，测试工程师3名。大专学历3人，本科学历4人，研究生学历1人。而两名带头的工程师均有8年以上行业经验，可以说是见证了高清行业的发展
                        <a href="javascript:;" style="color: #3a8ee6">>>more</a>
                    </p>
                    <!--<span>-->
                        <!--得益于雄厚的工程力量，公司在新品开发，产品改善，定制化工程案例等各方面均有完善成熟的项目体系，最大可能的做好产品售后服务，给客户注入了强大的信心!-->

                        <!--　　目前，公司所有的产品都已取得CE, FCC, RoHS 等国际测试认证，产品完全符合欧盟生产标准。我们的大屏商显、透明屏、安防监控设备等产品已广泛应用于酒店、商场、企业等展示场所，各大品牌电视机、投影机等显示设备生产厂家的测试中心以及像数据监控控制中心、高清信号分配转换应用中心、会议演示等各种工种之中!-->

                        <!--公司一直秉承以质量赢得口碑，因此也得到很多大型企业和个体的认可。河北省唐山市唐山银行安防工程由我公司铺设，自成立至今,凭借其雄厚的技术人才优势,先进的业务设备，更荣获河北省一级安防资质，金融行业备案证书！完善周到的服务与国内大型知名企业户建立了长期稳固的战略合作关系!-->

                        <!--　　展望未来，河北亿尔锐电子科技有限公司愿于广大合作伙伴一起携手共进，共创辉煌!-->
                    <!--</span>-->

                </div>

            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "xt-main",
        data(){
            return {

                showList: [
                    {
                        'background-image': 'url("../../assets/image/s1.png")'
                    },
                    {

                    },
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
