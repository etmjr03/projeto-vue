<template>
  <div class="header-dashboard">
    <span>Olá, {{ usuario.nome }}</span>
    <img src="../../assets/images/notificacao.svg" alt="teste">
  </div>
</template>

<script>
export default {
  data(){
    return {
      usuario: {
        nome: 'Usuário',
        perfil: 'Admin'
      }
    }
  }
}
</script>

<style>
  .header-dashboard{
    display: flex;
    width: 40%;
    height: 35px;
    padding: 10px;
    gap: 20px;
    justify-content: center;
    align-items: center;
    position: relative;

    background: #c9a8f5;
    border-radius: 30px;
  }

  .header-dashboard img {
    position: absolute;
    right: 10px;
  }

  @media only screen and (max-width: 800px) {
    .header-dashboard{
      width: 100%;
    }
  }
</style>