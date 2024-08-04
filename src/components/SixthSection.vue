<template>
    <div>
        <div class="row d-flex align-items-center justify-content-center margin-scoped">
            <div class="col-md-12">
                <div class="card position-relative">
                    <div class="card-body text-center d-flex align-items-center justify-content-center">
                        <div>
                            <img src="../assets/happy-person.png" class="card-img" alt="Foto da tradutora">
                        </div>
                        <div class="p-5">
                            <h5 class="title">Luciana Klai - Tradutora</h5>
                            <p class="card-text">Formada em Tradução e Interpretação pela Universidade Metodista de São
                                Paulo em 2011, atuo como tradutora especialista em resumos e artigos acadêmicos.</p>
                            <button class="btn-primar">SOLICITAR</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
img {
    max-height: 475px;
    width: auto;
    border-radius: 50%;
    min-width: 460px;
    object-fit: cover;
    border: 1px solid #d54dff;
    padding: 21px;
    background: #d54dff;
}
.title{
    font-size: 48px;
}

.card {
    min-height: 440px !important;
    border-radius: 20px;
    background-color: #2a2a2a !important;
    color: white;
    padding: 50px
}
.card-text{
    font-size: 28px;
}
</style>