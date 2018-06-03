<template>
<div id="two-app">
    <el-container>
        <el-aside width="180px">
          <el-card>
             <test-menu></test-menu>
          </el-card>
        </el-aside>
        <el-main>
          <el-card>
            <two></two>
          </el-card >
        </el-main>
    </el-container>
</div>
</template>

<script>
import TestMenu from "./TestMenu.vue"
import Two from "./two.vue"

export default {
  components: { Two,TestMenu },
    data() {
        return {
          
        }
    }
}
</script>

<style>
    .el-container{
      height: 97vh;
      border: 1px solid #eee;
    }
    .el-aside{
        background-color: #d3dce6;
        color:#333;
        line-height: 200px;
         
    }
    .el-main {
    background-color: #E9EEF3;
    color: #333;

    }
</style>


