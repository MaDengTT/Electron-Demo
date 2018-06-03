<template>
<div>    
    <el-button @click="open">这是按钮</el-button>
    <el-button type="primary" icon="el-icon-search">
        搜索
        </el-button> 
        <el-button type="primary" :loading="true">加载中</el-button>
</div>

</template>

<script>
export default {
    methods:{
        open(){
            const h = this.$createElement;
            this.$notify({
                title:'标题名称',
                message:h('i',{style:'color:teal'},"这时提示文案！！！")
            });
        }
    }
}
</script>


<style>

</style>
