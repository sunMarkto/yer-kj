<template>
    <el-container>
        <!--header-->
        <el-header>
            <xtHeader></xtHeader>
        </el-header>
        <!--main-->
        <el-main>
            <xtMain></xtMain>
        </el-main>
        <!--footer-->
        <el-footer>
            <xtFooter></xtFooter>
        </el-footer>
    </el-container>
</template>

<script>
    import xtHeader from '../components/xt-header'
    import xtMain from '../components/xt-main'
    import xtFooter from '../components/xt-footer'
	export default {
		name: "index",
        components: {
            xtHeader,
            xtMain,
            xtFooter,
        },
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
