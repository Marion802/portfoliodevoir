<template>
  <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playwrite+CU:wght@100..400&display=swap" rel="stylesheet">

<body class="fond">
      <header id="premierepartie" >
        <h1 class="uniquifier"> Marion SERMANDE </h1>
        <h2>Mon portfolio</h2>
        <!--mettre le  lien logo de l'entreprise -->
          <a href=""><img src="/src/assets/logo.cocoweb.png" alt="logo-entreprise-cocoweb" id="cocoweb"></a>
        <nav>
          <ul>
            <li> <a href="">Présentaion</a></li>
            <li> <a href="">Création</a></li>
            <li> <a href="">Formutaire de contact</a></li>
          </ul>
        </nav>
      </header>
      
      <main>
      
        <div id="present">
        <p>
          Je me présente Marion SERMANDE, heureuse fondatrice de COCO WEB. <br/>
          Specialiste du developpeur web, COCO WEB à été créer pour donner une image et de la visibilité a vos idées. <br/>
          Je vous laisse jeter un coup d'oeil sur les compétences acquises de COCO. 
        </p>
      </div>

      <div id="cv">
        <h3>CV en html</h3>
        <a href=""><img src="" alt=""></a>
      </div>

      <div id="cahierdescharges">
        <h3>Cahier des charges</h3>
        <a href=""><img src="" alt=""></a>
      </div>

      <div id="espacecomment">
        <h3>Dynamiser un espace commentaire</h3>
        <a href=""><img src="" alt=""></a>
      </div>


      <form action="#" method="post" id="formulaire">
        <h2>Contactez Coco</h2>
        <div>
          <label for="first-name">Prénom</label>
          <input type="text" name="first-name" id="first-name" value="first-name">
        </div>
        
        <div>
          <label for="last-name" >Nom</label>
            <input type="text" name="last-name" id="last-name">
        </div>
        
        <div>
          <label for="object" >Objet</label>
            <input type="text" name="object" id="object">
        </div>
        
        <div>
          <label for="message" >Commentaire</label>
          <textarea id="message" name="message" rows="4"  ></textarea>
        
        </div>
        <button type="submit"> Envoyer </button>
      </form>
    </main>

</body>


</template>




<script setup>
import pied from '@/App.vue'
</script>




<style scoped>

.uniquifier {
  font-family: "Playwrite CU";
  font-optical-sizing: auto;
  font-weight: 100;
  font-style: normal;
}



.fond {
  background-image: url(/src/assets/fond.png);
}



#cocoweb {
  width:150px ;
  height: 150px;
}
</style>
