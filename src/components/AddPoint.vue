<template>
    <div>
        <p>hello nihao</p>
        <p>{{ resultStr }}</p>
        <p @click="backBtnClick">fanhui zhy</p>      
    </div>
</template>
<script>
export default{
        components:{
                
        },
        data: () =>({
            resultStr: '',
        }),
        methods:{
              backBtnClick(){
                  this.$router.go(-1);
              }
        },
        created(){
                this.resultStr = this.$route.query.plan;
               
        },
        destroyed(){

        }
}
</script>
<style scoped>


</style>