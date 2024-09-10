<template>
  <div class="valores-dashboard">
    <div class="valores total">
      <p class="titulo-pedido">Total de pedidos</p>
      <p class="valor-pedido">R$ {{ valorPedidos }}</p>
      <p class="quantidade-pedido">Total pedidos: {{ quantidadePedidos }}</p>
    </div>
    <div class="valores">
      <p class="titulo-pedido">Pedidos aprovados</p>
      <p class="valor-pedido">R$ {{ valorAprovado }}</p>
      <p class="quantidade-pedido">Pedidos Aprovados: {{ quantidadePedidosAprovados }}</p>
    </div>
    <div class="valores">
      
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      quantidadePedidos: 3,
      quantidadePedidosAprovados: 1,
      valorPedidos: 300.50,
      valorAprovado: 100.35
    }
  }
}
</script>

<style>
  .valores-dashboard{
    display: flex;
    width: 100%;
    height: fit-content;
    margin-top: 20px;
    padding: 10px;
    align-content: center;
    flex-direction: column;
  }

  .valores{
    display: flex;
    width: 100%;
    height: 20vh;
    margin: 10px 0;
    padding: 10px;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 10px;
    
    background: #FFF;

    box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);
    -webkit-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);
    -moz-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);

    border-radius: 30px;
  }

  .titulo-pedido{
    font-size: 18px;
  }

  .valor-pedido{
    font-size: 30px;
    font-weight: 700;
    color: #fdc302;
  }

  .quantidade-pedido{
    font-size: 20px;
  }
</style>