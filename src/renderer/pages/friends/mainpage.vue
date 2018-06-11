<template>
    <div id="main">
        <el-container>
            <el-header height="60px">
                      <div id="icon" class="div-line">
                          <i class="el-icon-menu"></i>
                          </div>
                      <div id="title" class="div-line">WoelFel</div>
                      <div id="search" class="div-line">
                          <el-input size="small" v-model="input" placeholder="请输入内容">
                          </el-input>
                      </div>
                      <div id="right">
                          right name
                      </div>
            </el-header>
            <el-main>
                <div id="item-grid">
                    <div class="item" v-for="o in 10" :key="o">
                        <el-card class="box-card">
                            <div id="like">
                                like
                            </div>
                            <div id="itembody">
                                <img id="avatar" v-bind:src="testUrl">
                                <div id='name'> item {{o}}  Name </div>
                                <div id="info">Item {{o}}  .com</div>
                            </div>
                            <div id="bottom">
                                <div class="bottomdiv">Assign</div>
                                <div class="bottomdiv">Assign</div>
                            </div>
                        </el-card>
                    </div>
                </div>
            </el-main>
        </el-container>
    </div>
</template>

<script>
import testimg from '../../assets/header_icon_1.jpg';
export default {
    data(){
        return{
            input:'',
            testUrl:testimg,
            items:[
                {
                    imgUrl:testimg
                }
            ]
        }
    }
}
</script>
<style>
    body{
        background-color: #F5F7FA;
        margin: 0;
        padding: 0;
    }
    /* .el-container{
        width: 1600px;
    } */
    #icon{
        width: 40px;
        height: 40px;
        background-color: #ddd;
    }
    #title{
        margin-left: 20px;
        font-size: 20;
        color: #5B6378;
    }
    #search{
        margin-left: 60px;
    }
    #right{
        float: right;
    }
    #like{
        float: right;
    }
    .el-header{
        background-color: #fff;
        line-height: 60px;
        box-shadow: 0px 1px 1px 0px #e2e0e0;
    }
    .el-col{
        background-color: #ccc
    }
    .div-line{
        float: left;
    }
    .item{
        float: left;
        margin-left: 24px;
        margin-top: 24px;

    }
    .box-card{
        width: 304px;
        height: 360px;
    }
    #itembody{
        float: right;
        width: 100%;
        text-align: center;
    }
    img#avatar {
    width: 120px;
    height: 120px;
    border-radius: 100px;
    margin-top: 30px;
    }
    div#name {
    font-size: 18px;
    color: #000;
    font-family: 微软雅黑;
    margin-top: 16px;
}


div#info {
    font-size: 14px;
    color: #98A0A6;
    margin-top: 16px;
}
div#bottom {
    width: 100%;
    float: right;
    position: relative;
    margin-top: 24px;
}
.bottomdiv {
    float: right;
    width: 50%;
    color: #98A0A6;
    font-size: 14px;
}
</style>

