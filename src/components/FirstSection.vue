<template>
    <div class="banner container d-flex align-items-center w-100 justify-content-between">
      <div class="banner-content">
        <h1>Tradução Profissional de <i>Abstract</i> Acadêmico</h1>
        <p>Garanta a fidedignidade do seu trabalho acadêmico para a comunidade internacional.</p>
        <button>SOLICITAR</button>
      </div>
      <div class="banner-image position-relative">
        <div class="bg-gradient">
        </div>
        <div>
          <img src="../assets/happy-person.png" alt="">
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .banner {
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: #fff;
    padding: 50px;
  }
  .banner-image{
    max-width: 420px;
    object-fit: cover;
  }
  .bg-gradient{
    background-color: #d54dff;
    width: 100%;
    position: absolute;
    height: 100%;
    z-index: -1;
    filter: blur(50px) !important;
    clip-path: polygon(75% 0%, 100% 50%, 75% 100%, 0% 100%, 25% 50%, 0% 0%);
  
  }
  .banner-content h1 {
    font-size: 3rem;
    font-weight: bold;
    margin-bottom: 20px;
  }
  
  .banner-content p {
    font-size: 1.2rem;
    margin-bottom: 40px;
  }
  
  .banner-content button {
    background-color: #d54dff;
    color: #fff;
    border: none;
    padding: 7px 30px;
    border-radius: 30px;
    cursor: pointer;
    font-size: 1.2rem;
    transition: background-color 0.3s ease;
  }
  
  .banner-content button:hover {
    background-color: #c03be0;
  }
  
  </style>
  