<template>
    <div class = "hd">
        <div class="U-head">
            <div class = "logo">
                <p style="padding-top :20px">XX科技</p>
            </div>
            <div class = "header-content">
                <br>
                <p>首页&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;产品中心
                    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;新闻动态
                     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;关于公司
                     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;联系我们
                     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;招聘信息
                </p>
                <el-menu
                            :default-active="activeIndex2"
                            class="el-menu-demo"
                            mode="horizontal"
                            @select="handleSelect"
                            text-color="#fff"
                            background-color="rgb(57, 118, 223)"
                    >
                    <el-menu-item index = "2">
                        <a>首页</a>
                    </el-menu-item>
                    <el-menu-item index = "3">
                        <a>产品中心</a>
                    </el-menu-item>
                    <el-menu-item index = "4">
                        <a>新闻动态</a>
                    </el-menu-item>
                    <el-menu-item index = "5">
                        <a>关于公司</a>
                    </el-menu-item>
                    <el-menu-item index = "6">
                        <a>联系我们</a>
                    </el-menu-item>
                    <el-menu-item index = "7">
                        <a>招聘信息</a>
                    </el-menu-item>
                </el-menu>
            </div>
            <div class="header-right">
                    <a style="height: 90px;line-height: 90px">
                        登陆
                    </a>|
                    <a style="height: 90px;line-height: 90px">
                        注册
                    </a>
            </div>
        </div>
    </div>
</template>
<script>
    export default {
        data() {
            return {
                activeIndex: '1',
                activeIndex2: '1'
            };
        },
        methods: {
            handleSelect(key, keyPath) {
                console.log(key, keyPath);
            }
        }
    }
</script>

<style>
    .hd{
        width:100%;
        height:90px;
        background-color: rgb(0, 0, 0);
        position: relative;
        z-index: 1000;
        left: 0;
        top:0;
        overflow: hidden;
    }
    .U-head {
        padding: 0 30px;
        height: 100%;

    }
    .logo{
        width:220px;
        float: left;
        height: 100%;
    }
    .header-content{
        width: 60%;
        float: left;
        height: 100%;
        padding-left: 60px;
    }
    .header-right{
        width: 9%;
        float: left;
        height: 100%;
    }
    .el-menu-demo{
        color: rgb(255, 255, 255) !important;
        height: 90px;
        line-height: 90px;
        text-decoration: none;
        font-size: 18px;
    }
</style>