<template>
     <section class="container py-3 apropos ">
      <div class="carte row my-3 mx-2 p-5">
        <div class="apropos_presentation col-md-6 ">
          <div class="apropos " id="apropos">
            <h3 class="titres ">À propos</h3>
          </div>
          <div class="paragraphe mt-3">
            <p>
              Passionné par l'informatique et des nouvelles technologie, je suit actuellement
              une fomation de <strong>développeur web</strong> au seins du centre européen de
              formation (CEF). J'ai acquis depuis le debut de cette formation de nombreuses
              bases solides afin de pouvoir travailler dans le domaine du <strong>développement</strong>.
            </p>
            <p>
              Basé à Lyon, je suis à la recherche d'un stage de <strong>10 semaines minimum</strong> au sein d'une
              entreprise pour validier mon
              diplome et approfondir mes connaissance dans le domaine du <strong>développement web et web
                mobile</strong>.
            </p>
            <p>
              J'accorde une attention particulière à la qualité du code que j'écris et je
              respecte les bonnes pratiques du web.
            </p>
          </div>
        </div>

        <div class="col-md-6">
          <img src="" alt="Samuel VIVIER">
          <div class="hard-skills">
            <h3 class="titres">Hard Skills</h3>

            <div class="logo">
              <img src="../assets/images/html-5.png" alt="Html5">
              <img src="../assets/images/css-3.png" alt="CSS3">
              <img src="../assets/images/js.png" alt="JavaScript">
              <img src="../assets/images/git.png" alt="Git">
              <img src="../assets/images/github.png" alt="Github">
              <img src="../assets/images/vue.jpg" alt="Vue.js">
              <img src="../assets/images/react.jpg" alt="React">
              <img src="../assets/images/angular.jpg" alt="Angular">
            </div>

          </div>
        </div>
      </div>
    </section>
</template>

<script setup>
</script>

<style scoped>


.carte {
    border-radius: 10px;
    background-color: #f1fffa;
}

.logo{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}
.logo img{
    max-width: 25%;
    margin: 10px;
    width: 100px;
    height: 100px;
    border-radius:25px ;
}
.titres{
    font-family: "Playfair Display", serif;
}
p{
    font-family: "Montserrat", sans-serif;
}
.apropos{
    /* display: none; */
}
</style>