<template>
  <div>
      <!-- <button class="btn btn-fixed" data-bs-toggle="modal" @click="toggleReturn" data-bs-target="#exampleModalToggle">Inscreva-se <span><img
        class="arrow" src="./Arrow1.png" alt=""></span></button> -->
      <header>
          <nav class="navbar navbar-expand-lg menu">
              <div class="container d-flex justify-content-between">
                  <a class="navbar-brand" href="https://creators.llc/" target="_blank">
                      <img class="logo_asset" src="../assets/logo.JPG" alt="">
                  </a>
                  <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarMenu"
                      aria-expanded="false" aria-label="Toggle navigation">
                      <span class="navbar-toggler-icon"></span>
                  </button>

                  <div class="collapse navbar-collapse" id="navbarMenu">
                      <ul class="navbar-nav">
                          <li class="nav-item">
                              <a class="nav-link" href="#como-funciona">Aulas</a>
                          </li>
                          <li class="nav-item">
                              <a class="nav-link" href="#como-participar">Cursos Gravados</a>
                          </li>
                          <!-- <li class="nav-item">
                              <a class="nav-link" href="#">Mentores</a>
                          </li> -->
                          <li class="nav-item">
                              <a class="nav-link" href="#programacao">Livros</a>
                          </li>
                          <li class="nav-item">
                              <a class="nav-link" href="#faq">Atividades</a>
                          </li>
                          <li class="nav-item">
                              <a class="nav-link" href="#faq">Blog</a>
                          </li>
                          <li class="nav-item">
                              <a class="nav-link" href="#faq">Abstract</a>
                          </li>
                          <li class="nav-item">
                              <a class="nav-link" href="#faq">Sobre</a>
                          </li>
                          <li class="nav-item">
                              <a class="nav-link" href="#faq">For Teachers</a>
                          </li>
                          <li class="nav-item">
                              <a class="btn-primary" href="#faq">Login</a>
                          </li>
                      
                      </ul>
                  </div>
              </div>
          </nav>
      </header>
      <section class="main-section position-relative">
          <div class="row">
              <div class="col-md-6 info">
                  <div>
                      <h1>APRENDIZADO <br> ESTRATÉGICO</h1>
                      <p>Aprenda por meio de situações do dia a dia, tornando o aprendizado <br> mais prático e eficiente. Vai fazer aquela entrevista em inglês ou está <br> precisando de ajuda para sua apresentação no trabalho?  <br>
                          <strong>Vamos praticar!</strong>
                      </p>                   
                  </div>
              </div>
              <div class="col-md-6">
                  <img class="people position-absolute bottom-0 end-0" src="../assets/happy-person.png" alt="">
              </div>
          </div>
      </section>
      <main>
          <div class="container" id="como-funciona">
              <h2 class="margin-section">Por que escolher a Klai?</h2>
              <div class="card" v-for="(item, index) in items" :key="index">
                  <div class="row d-flex align-items-center">
                      <div class="col-md-6 img-star d-flex align-items-center justify-content-center"><img
                              :src="item.image" alt=""></div>
                      <div class="col-md-6 info">
                          <h2 class="item-title"><span class="me-3"><img :src="item.numbers" alt=""></span>{{
                              item.title }}
                          </h2>
                          <p class="item-description" v-html="item.description"></p>
                      </div>
                  </div>
              </div>
              <h2 class="margin-section" id="como-participar">Como participar do programa AliExperts</h2>
              <div class="card" v-for="(item, index) in itemsWork" :key="index">
                  <div class="row d-flex align-items-center">
                      <div class="col-md-6 img-star d-flex align-items-center justify-content-center"><img
                              :src="item.image" alt=""></div>
                      <div class="col-md-6 info">
                          <p class="item-description" v-html="item.description"></p>
                      </div>
                  </div>
              </div>
          </div>
          <div class="container">
              <div class="row">
                  <div v-for="(item, index) in itemsMiniCard" :key="index" class="col-md-6 col-sm-3">
                      <div class="mini-card">
                          <span class="me-4"><img src="./losango.svg" alt=""></span>
                          <h6 class="mb-5" v-html="item.content"></h6>
                          <p v-html="item.text"></p>
                      </div>
                  </div>
              </div>
          </div>
       
          <!-- <div class="container" id="programacao">
              <h2 class="margin-section">Conteúdo educacional do AliExperts</h2>
              <div class="row d-flex justify-content-center card-part">
                  <div v-for="(item, index) in cards" :key="index" class="col-md card-educational">
                      <div class="text-center alignment">
                          <span class="item-number-card">{{item.numbers}}</span>
                          <p class="mt-5" v-html="item.description"></p>
                      </div>
                  </div>
              </div>
          </div> -->
          <!-- <div class="container" id="faq">
              <h2 class="margin-section">FAQ</h2>
              <div class="container">
                  <div class="row">
                      <div class="col-md-12">
                          <div v-for="(item, index) in accordionItems" :key="index" class="accordion-item">
                              <div @click="toggleAccordion(index)" class="accordion-header">
                                  {{ item.title }}
                                  <span :class="{ 'rotate-arrow': activeIndex === index }">&#9660;</span>
                              </div>
                              <div v-if="activeIndex === index" class="accordion-content" v-html="item.content"></div>
                          </div>                          
                      </div>
                  </div>
              </div>
          </div> -->
      </main>
      <div class="margin-section"></div>
      <footer class="text-dark">
          <div class="container">
              <div class="row d-flex align-items-center justify-content-between">
                  <div class="col-md-6">
                      <div>
                          <ul class="list-unstyled d-flex gap-4">
                              <li><a href="#como-funciona">Como funciona</a></li>
                              <li><a href="#como-participar">Como participar</a></li>
                              <li><a href="#programacao">Programação</a></li>
                              <li><a href="#faq">FAQ</a></li>
                          </ul>
                      </div>
                  </div>
                  <div class="col-md-6 text-md-end">
                    <img class="logo_asset" src="../assets/logo.JPG" alt="">
                      <p class="mt-3 email">Fale conosco | <a href="mailto:hello@creators.llc">klaienglish@gmail.com</a>
                      </p>
                  </div>
              </div>
          </div>
      </footer>   
  </div>
</template>
<script>
export default {
  data() {
    return {
      activeIndex: null,
      creatorsForm: false,
      accordionItems: [
        {
          title: 'Quantos produtos serão enviados? Precisa devolver?',
          content: 'Será enviado pelo menos 1 produto mensal, não é necessária a devolução.'
        },
        {
          title: 'Como funciona o comissionamento?',
          content: 'Saiba todas as regras de comissionamento neste link: <a href="https://learning.br.aliexpress.com/course/learn?id=2623&type=video&spm=courserlist_courses.4.0">Programa de Afiliados do AliExpress</a>'
        },
        {
          title: 'Qual o critério de avaliação dos conteúdos para a bonificação?',
          content: 'Criatividade, performance, engajamento, entrega completa de acordo com o briefing, agilidade, retorno em vendas, entre outros.'
        },
        {
          title: 'Haverá um cronograma de postagem pré-definido?',
          content: 'Sim, ela será compartilhada com os criadores a cada briefing enviado.'
        },
        {
          title: 'A participação nas aulas é obrigatória? Será calculada a frequência?',
          content: 'A participação é recomendada, mas não obrigatória. As aulas também ficarão gravadas para o consumo posterior, caso você não consiga assistir ao vivo.'
        },
        {
          title: 'O pagamento está vinculado à performance apenas ou tem um valor fixo? Como é feito o pagamento?',
          content: 'O pagamento de comissionamento é vinculado à performance. O pagamento dos desafios tem um valor fixo que será enviado junto ao briefing. O pagamento é realizado através de invoice internacional e você recebe na conta indicada na plataforma da Creators.llc, na área de dados bancários.'
        },
        {
          title: 'Vou precisar ter exclusividade com a AliExpress ou posso indicar produtos da concorrência?',
          content: 'Não há exclusividade, mas quanto mais produtos da mesma plataforma você indicar, melhores são as suas chances de monetização.'
        },
        {
          title: 'Qual a duração do projeto?',
          content: 'Não há previsão de encerramento, enquanto você entregar conteúdos no programa, o comissionamento estará ativo.'
        },
      ],
      items: [
        {
          numbers: "./2.svg",
          title: "Trilhas Personalizadas",
          image: "../Group527.png",
          description: "As aulas são cuidadosamente preparadas para atender às necessidades individuais de cada aluno, por meio de trilhas de aprendizado exclusivas e metas individuais para cada diferente estilo de aprendizado.",
        },
        {
          numbers: "./22.svg",
          title: "Aprendizado Estratégico",
          image: "./Group539.png",
          description: "Aprenda por meio de situações do dia a dia, tornando o aprendizado mais prático e eficiente. Vai fazer aquela entrevista em inglês ou está precisando de ajuda para sua apresentação no trabalho? Vamos praticar!",
        },
        {
          numbers: "./4.svg",
          title: "Feedbacks Recorrentes",
          image: "./Group528.png",
          description: "Feedbacks regulares, destacando suas conquistas e apontando maneiras específicas para que você possa avançar, moldando o caminho de acordo com suas necessidades.",
        },
       
      ],
      cards: [
        {
          numbers: "01",
          description: "Posicionamento estratégico e performance",
        },
        {
          numbers: "02",
          description: "Identidade visual <br> no conteúdo",
        },
        {
          numbers: "03",
          description: "Contando história <br> através  de ganchos",
        },
        {
          numbers: "04",
          description: "Técnicas de edição de vídeos, takes e cortes",
        },
        {
          numbers: "05",
          description: "Como identificar e metrificar seus resultados",
        },
      ],
      itemsWork: [
        {
          image: "./Group544.png",
          description: "4 Técnicas Inovadoras para Turbinar Sua Fluência em Inglês <br/><br/><br/> Dominar um novo idioma é uma jornada emocionante, mas às vezes desafiadora. A busca pela fluência em inglês pode ser transformada em uma experiência envolvente e eficaz ao incorporar técnicas inovadoras ao seu aprendizado. Neste artigo, exploraremos quatro abordagens diferenciadas que não apenas tornarão sua jornada de aprendizado mais empolgante, mas também irão impulsionar significativamente sua fluência no inglês. Está pronto para uma revolução no seu aprendizado de inglês? Vamos começar!"
        }
      ],
      itemsMiniCard: [
        { content: '1 – Aprendizado por Gamificação:', text: 'Explore aplicativos e plataformas que incorporam elementos de jogos para tornar o aprendizado mais envolvente. Exemplo: Duolingo – Um aplicativo que utiliza elementos de jogos para tornar o aprendizado de idiomas divertido e interativo. Os usuários ganham pontos e avançam de nível à medida que completam lições.' },
        { content: '2 – Conversação com Inteligência Artificial:', text: 'Descubra as vantagens de utilizar assistentes de voz, como Siri, Google Assistant ou Amazon Alexa, para praticar conversação. Eles podem ajudar na pronúncia e compreensão auditiva. Exemplo: Google Assistant – Use comandos de voz para realizar atividades diárias e pratique frases e perguntas com a assistência da IA. A função de tradução também pode ser útil.' },
        { content: '3 – Realidade Virtual para Simulações de Conversação:', text: 'Investigação de recursos de realidade virtual que oferecem ambientes simulados para prática de conversação. Plataformas como Engage VR podem proporcionar experiências imersivas. Plataforma: AltspaceVR – Oferece eventos virtuais e salas de bate-papo onde você pode praticar conversação em inglês com pessoas de todo o mundo em ambientes virtuais.' },
        { content: '4 – Métodos de Aprendizado Baseados em Música:', text: 'Explore técnicas que incorporam música ao aprendizado, como letras de músicas, karaokê ou até mesmo a criação de suas próprias canções para memorizar vocabulário e melhorar a pronúncia. Atividade: Karaoke com Letras em Inglês – Participe de sessões de karaokê online ou use aplicativos que exibem as letras enquanto você canta. Isso ajuda na pronúncia e no vocabulário.' },
      ],
      tutors: [
        {
          image: "./Group155.png",
          name: "@nome da influencer aqui",
          description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic cupiditate nulla voluptatem  nostrum tenetur libero inventore consequatur aut necessitatibus assumenda fugit!"
        },
        {
          image: "./Group156.png",
          name: "@nome da influencer aqui",
          description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic cupiditate nulla voluptatem natus error, unde obcaecati ad eveniet id blanditiis pariatur nostrum tenetur libero inventore consequatur aut necessitatibus assumenda fugit!"
        },
        {
          image: "./Group157.png",
          name: "@nome da influencer aqui",
          description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic cupiditate nulla voluptatem natus error, unde obcaecati ad eveniet id blanditiis pariatur nostrum tenetur libero inventore consequatur aut necessitatibus assumenda fugit!"
        },
        {
          image: "./Group155.png",
          name: "@nome da influencer aqui",
          description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic cupiditate nulla voluptatem natus error, unde obcaecati ad eveniet id blanditiis pariatur nostrum tenetur libero inventore consequatur aut necessitatibus assumenda fugit!"
        },
        {
          image: "./Group155.png",
          name: "@nome da influencer aqui",
          description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic cupiditate nulla voluptatem natus error, unde obcaecati ad eveniet id blanditiis pariatur nostrum tenetur libero inventore consequatur aut necessitatibus assumenda fugit!"
        },
        {
          image: "./Group155.png",
          name: "@nome da influencer aqui",
          description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic cupiditate nulla voluptatem natus error, unde obcaecati ad eveniet id blanditiis pariatur nostrum tenetur libero inventore consequatur aut necessitatibus assumenda fugit!"
        },
      ],
      formData: {
        name: "",
        email: "",
        password: "",
        phone: "",
        perfil: "",
        origin: "aliexperts",
        date_subscription: "",
        specialities: [],
        validacaoRedes: [
          { socialMedia: '', link: '' }
        ]
      },
      passwordStrength: '',
      showingTooltip: false,
      isLoading: false,
      success: '',
      error: '',
      selectedCount: 0,
      selectedSocialMedia: '',
      socialMediaInput: '',
      showAllFields: true,

      vertical: [
        { name: "Beleza", id: 263 },
        { name: "Casa", id: 306 },
        { name: "Decoração", id: 307 },
        { name: "Esporte", id: 305 },
        { name: "Fitness", id: 264 },
        { name: "Games", id: 362 },
        { name: "Moda", id: 323 },
        { name: "Tecnologia", id: 368 },
      ],
    }
  },

  methods: {
  }
}
</script>
