<template>
  <div class="dashboard">
    <HeaderDashboardComponent/>
    <ValorComponent/>
  </div>
</template>

<script>
import HeaderDashboardComponent from './header/HeaderDashboardComponent.vue';
import ValorComponent from './valores/ValorComponent.vue';

export default {
  components: {
    HeaderDashboardComponent,
    ValorComponent
  }
}
</script>

<style>
  .dashboard{
    width: 88%;
    height: 88vh;
    margin: 20px auto;
    padding: 10px;

    background: rgba(255, 255, 255, 0.26);
    box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(6.1px);
    -webkit-backdrop-filter: blur(6.1px);
    border: 2px solid rgba(255, 255, 255, 0.3);

    box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);
    -webkit-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);
    -moz-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);

    border-radius: 30px;
  }
</style>