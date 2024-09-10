<template>
  <HeaderComponent/>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent
  }
}
</script>

<style>
body{
  height: 100vh;
  overflow: hidden;
  background: #c9a8f5;
  background: linear-gradient(135deg, #c9a8f5 0%, #0e74f1 88%, #009ddb 100%);
  background: -moz-linear-gradient(135deg, #c9a8f5 0%, #57a0fa 88%, #009ddb 100%);
  background: -webkit-linear-gradient(135deg, #c9a8f5 0%, #0e74f1 88%, #009ddb 100%);
  filter: progid: DXImageTransform.Microsoft.gradient( startColorstr="#CAA8F5", endColorstr="#1075f1", GradientType=1 );
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 10px;
}

@media only screen and (max-width: 800px) {
  body{
    background: #FFF;
  }
}
</style>
