<template>
  <div id="app">
    <img src="./assets/logo.png">
    <ul>
      <li v-for="book in books">
        <a v-bind:href="book.url">{{book.name }}</a>
      </li>  
    </ul>
    
  </div>
</template>

<script>
module.exports={
  data:function(){
    return  {
      msg: 'hello Vue.JS!22222'+new Date(),
      seen:false,
      books:[{name:'Java',url:'http://www.163.com'},
        {name:'Oracle',url:'http://www.baidu.com'},
        {name:'NodeJS',url:'http://www.sohu.com'}]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
