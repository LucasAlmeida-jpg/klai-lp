<template>
    <div class="abstract d-flex justify-content-center">
        <div>
            <h1 class="highlight text-center margin-scoped-bottom">O que é um Abstract?</h1>
            <p>O <i>abstract</i> é a tradução para uma língua estrangeira do resumo de sua pesquisa.</p>
            <p>Trata-se de um componente essencial nos elementos pré-textuais de trabalhos científicos, incluindo
                monografias, dissertações e teses.</p>
            <p>Em relação a artigos, ele é considerado um elemento obrigatório pela maioria dos periódicos.</p>
            <p>Quando redigir um <i>abstract</i>, é crucial incorporar todas as informações contidas no resumo original.
                Dessa forma, o <i>abstract</i> deve abranger:</p>
            <p v-for="(item, index) in abstract" :key="index" class="d-flex align-items-center gap-2 list">
                <img src="../assets/joinha.svg" alt="ok">
                <span>{{ item }}</span>
            </p>
            <p>Para assegurar precisão e qualidade, com a Klai você conta com um tradutor especializado para converter o
                seu Resumo (Português) para o <i>Abstract</i> (Inglês).</p>

        </div>
    </div>
    <div class="d-flex justify-content-center align-items-center mt-3 margin-scoped-bottom">
        <button class="btn-primar">SOLICITAR</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            abstract: [
                'A apresentação do objeto de investigação',
                'O estabelecimento do objetivo geral',
                'A descrição da metodologia empregada',
                'A indicação dos principais resultados obtidos'
            ]
        }
    },
    methods: {

    }
}
</script>

<style scoped>
.abstract {
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


.list {
    list-style: none !important;
}

</style>