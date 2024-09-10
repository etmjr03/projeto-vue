<template>
  <div 
    class="menu-principal" 
    :class="{'esconder-menu-mobile': exibirMenuMobile}"
  >
    <div class="itens-menu">Início</div>
    <div class="itens-menu">Produtos</div>
    <div class="itens-menu">Clientes</div>
    <div class="itens-menu">Pedidos</div>
  </div>
  <div @click="exibirMenu" class="item-menu-responsivo">
    <img src="../assets/images/config.svg" alt="">
  </div>
</template>

<script>
export default {
  data(){
    return {
      exibirMenuMobile: true
    }
  },
  methods: {
    exibirMenu(){
      this.exibirMenuMobile 
        ? this.exibirMenuMobile = false 
        : this.exibirMenuMobile = true 
    }
  }
}
</script>

<style>
  .menu-principal{
    display: flex;
    width: 750px;
    height: 50px;
    margin: 0 auto;
    justify-content: center;
    align-items: center;
    gap: 20px;
    
    background: rgba(255, 255, 255, 0.26);
    border-radius: 16px;
    box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(6.1px);
    -webkit-backdrop-filter: blur(6.1px);
    border: 2px solid rgba(255, 255, 255, 0.3);

    box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);
    -webkit-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);
    -moz-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);

    border-radius: 30px;
  }

  .itens-menu{
    display: flex;
    width: 100px;
    height: 80%;
    justify-content: center;
    align-items: center;
    border-radius: 20px;
    cursor: pointer;

    color: #FFF;
    font-weight: 700;
  }

  .itens-menu:hover{
    color: #000;
  }

  .item-menu-responsivo{
    display: none;
    width: 50px;
    height: 50px;
    padding: 10px;
    text-align: center;

    background: #0e74f1;

    box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);
    -webkit-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);
    -moz-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);

    cursor: pointer;
    border-radius: 50%;
  }

  @media only screen and (max-width: 800px) {
  .menu-principal{
    width: fit-content;
    height: fit-content;
    flex-direction: column;
    position: absolute;
    top: 100px;
    
    box-shadow: none;
  }

  .itens-menu{
    height: 50px;
    color: #000;
  }

  .item-menu-responsivo{
    display: flex;
    margin-top: 10px;
  }

  .esconder-menu-mobile{
    display: none;
  }
}
</style>