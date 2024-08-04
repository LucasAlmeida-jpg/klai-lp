<template>
    <div class="importance-container">
      <h1 class="title">A importância de um abstract fidedigno:</h1>
      <div class="importance-content">
        <div v-for="(item, index) in items" :key="index" class="importance-item">
            <img class="col-2" src="../assets/joinha.svg" alt="ok">
          <h3 class="mt-3">{{ item.title }}</h3>
          <p>{{ item.description }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        items: [
          {
            title: 'Comunicação efetiva',
            description: 'A fidedignidade do abstract é crucial para uma comunicação efetiva entre os pesquisadores e a comunidade acadêmica internacional. Ao garantir a precisão na tradução do resumo, os leitores estrangeiros conseguem compreender completamente a essência da pesquisa, promovendo a troca de conhecimentos e a colaboração internacional.'
          },
          {
            title: 'Avaliação Justa e precisa',
            description: 'A confiabilidade do abstract traz garantia de uma avaliação justa e precisa por parte de revisores e comitês editoriais. Uma tradução precisa assegura que o trabalho seja avaliado pelo seu mérito científico real, sem distorções causadas por erros de interpretação ou tradução.'
          },
          {
            title: 'Reputação acadêmica',
            description: 'Um abstract fidedigno desempenha um papel fundamental na construção da reputação acadêmica do autor e da instituição. Abstracts precisos e bem traduzidos refletem um comprometimento com a excelência acadêmica, contribuindo para a credibilidade do pesquisador e fortalecendo a posição da instituição no cenário internacional.'
          }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .importance-container {
    text-align: center;
    color: #b19dd8;
  }
  
  .importance-content {
    display: flex;
    justify-content: space-around;
    align-items: flex-start;
    flex-wrap: wrap;
  }
  
  .importance-item {
    background-color: #2a2a2a;
    border-radius: 10px;
    padding: 20px;
    margin: 10px;
    flex: 1;
    text-align: center;
    color: #ffffff;
    min-height: 366px !important;
  }
  
  .importance-icon {
    display: block;
    margin: 0 auto 20px;
    width: 50px;
    height: 50px;
  }
  
  h3 {
    font-size: 1.5em;
    margin-bottom: 10px;
  }
  
  p {
    font-size: 1em;
  }
  </style>
  