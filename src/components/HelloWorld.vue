<template>
  <div class="hello">
    <h2>Essential Links</h2> 
    <button @click="btnclick">点击跳转</button>   
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: () =>({
       resultStr: 'loading...',
  }),
  methods:{
    btnclick(){
     
      this.$router&&this.$router.push({
            path: 'AddPoint', 
            query: { plan: '123' }
        })
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
