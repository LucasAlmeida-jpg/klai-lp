<template>
    <div class="translator-container">
      <div class="overlay"></div>
      <div class="content">
        <h1 class="title">Por que escolher um tradutor profissional?</h1>
        <p class="description">
          A tradução e revisão do abstract por um tradutor profissional garantem que seu trabalho acadêmico seja corretamente interpretado e respeitado pela comunidade internacional. A precisão na tradução é crucial para a credibilidade e impacto do seu trabalho.
        </p>
        <button class="btn-primar">SOLICITAR</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {};
    },
    methods: {
        //
    },
  };
  </script>
  
  <style scoped>
  .translator-container {
    position: relative;
    text-align: center;
    color: white;
    background-size: cover;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .content {
    position: relative;
    z-index: 1;
    max-width: 800px;
    padding: 20px;
  }
  
  .description {
    font-size: 1.2em;
    margin-bottom: 40px;
  }
  
  </style>
  