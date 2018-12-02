<template>
    <el-container>
        <el-header class="header">
            <div class="header-wrap">
                <div class="header-logo">

                </div>
                <div class="header-drop">

                </div>
            </div>
        </el-header>
        <el-main>Main</el-main>
        <el-footer>Footer</el-footer>
    </el-container>
</template>

<script>
	export default {
		name: "index",
        data(){
		    return {

            }
        },
        methods: {

        }
	}
</script>

<style scoped>
    .header-wrap{
        margin: 0 auto;
        width: 65%;
        height: 60px;
        justify-content: space-between;
    }
    .header-logo{
        display: inline-block;
        height: 100%;
        width: 320px;
        background-color: #404241;
    }
    .header-drop{
        display: inline-block;
        height: 100%;
        width: 600px;
        background-color: black;
    }
</style>
