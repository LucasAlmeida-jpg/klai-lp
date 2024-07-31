<template>
    <div class="abstract-container d-flex align-items-center justify-content-center">
        <div>
            <h1>O que é um <span class="highlight">Abstract?</span></h1>
            <p>O <i>abstract</i> é a tradução para uma língua estrangeira do resumo de sua pesquisa.</p>
            <p>Trata-se de um componente essencial nos elementos pré-textuais de trabalhos científicos, incluindo
                monografias, dissertações e teses.</p>
            <p>Em relação a artigos, ele é considerado um elemento obrigatório pela maioria dos periódicos.</p>
            <p>Quando redigir um <i>abstract</i>, é crucial incorporar todas as informações contidas no resumo original.
                Dessa forma, o <i>abstract</i> deve abranger:</p>
            <ul>
                <li>Uma introdução concisa;</li>
                <li>A apresentação do objeto de investigação;</li>
                <li>O estabelecimento do objetivo geral;</li>
                <li>A descrição da metodologia empregada;</li>
                <li>Uma indicação dos principais resultados obtidos.</li>
            </ul>
            <p>Para assegurar precisão e qualidade, com a Klai você conta com um tradutor especializado para converter o
                seu Resumo (Português) para o <i>Abstract</i> (Inglês).</p>
            <button class="btn">SOLICITAR</button>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
      
    }
}
</script>

<style scoped>
.abstract-container {
    color: white;
}

.highlight {
    color: #e08eff;
}

ul {
    text-align: left;
    list-style: none;
    padding: 0;
}

li::before {
    content: '• ';
    color: white;
}

button {
    background-color: #d54dff;
    color: #fff;
    border: none;
    padding: 7px 30px;
    border-radius: 30px;
    cursor: pointer;
    font-size: 1.2rem;
    transition: background-color 0.3s ease;
}

button:hover {
    background-color: #d057e0;
}
</style>