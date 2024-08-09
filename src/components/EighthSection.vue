<template>
    <div class="promo-card">
        <h1 class="title text-center">Valor Promocional 2º Sem 2024</h1>
        <div class="promo-content d-flex justify-content-center">
            <div>
                <h2>Tradução de Resumo Acadêmico (Abstract)</h2>
                <ul>
                    <li>Tenha seu <i>abstract</i> traduzido pra você por um especialista;</li>
                    <li>Fique tranquilo e receba uma tradução precisa e confiável;</li>
                    <li>Receba seu <i>abstract</i> de forma rápida (5 dias úteis).</li>
                </ul>
                <div class="price">
                    <p class="old-price">De: <span>R$107,00</span></p>
                    <p class="new-price">Por: <span>R$89,90</span></p>
                </div>
                <p class="note">⚠️ não inclui revisão acadêmica ou formatação ABNT</p>
                <img src="../assets/happy-person.png" alt="Graduate" class="student-img">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "PromoCard",
};
</script>

<style scoped>
.promo-card {
    text-align: center;
}

.promo-content {
    background-color: #2a2a2a;
    color: white;
    padding: 55px;
    border-radius: 10px;
    margin: 20px auto;
    max-width: 500px;
    position: relative;
}


h2 {
    font-size: 20px;
    margin-bottom: 10px;
    text-align: left;

}

ul {
    list-style-type: none;
    padding: 0;
    text-align: left;
}

li {
    margin-bottom: 10px;
}

.price {
    margin: 20px 0;
    font-size: 18px;
}

.old-price span {
    text-decoration: line-through;
    color: red;
}

.new-price span {
    font-size: 32px;
    color: #9a47e4;
}

.note {
    font-size: 12px;
    color: gray;
}

.btn {
    background-color: #9a47e4;
    color: white;
    border: none;
    padding: 10px 20px;
    font-size: 16px;
    border-radius: 5px;
    cursor: pointer;
}

.btn:hover {
    background-color: #822dbf;
}

.student-img {
    width: 150px;
    margin-top: 20px;
    position: absolute;
    bottom: 0px;
    right: -53px;
}
</style>