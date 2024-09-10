<template>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Kanit:wght@600&display=swap" rel="stylesheet">


      <header id="premierepartie" >
        <div class="titre">
        <h1 class="kanit-semibold"> Marion SERMANDE </h1>
        
        
        <!--mettre le  lien logo de l'entreprise -->
          <a href="#"><img src="/src/assets/logo.cocoweb.png" alt="logo-entreprise-cocoweb" id="cocoweb"></a>
        </div>
        <div class="nav">
          <img src="/src/assets/souris.png" alt="une souris d'ordinateur rose" id="souris">
          <nav class="kanit-semibold" id="navi">
          <ul>
            <li> <a href="#present">Présentation</a></li>
            <li> <a href="#crea">Création</a></li>
            <li> <a href="#formulaire">Formutaire de contact</a></li>
          </ul>
        </nav>
        </div>
      </header>
    <body class="fond">
      <main>
      
        <div id="present">
        <p>
          Je me présente Marion SERMANDE, heureuse fondatrice de COCO WEB. <br/>
          Specialiste du developpeur web, COCO WEB à été créer pour donner une image et de la visibilité a vos idées. <br/>
          Je vous laisse jeter un coup d'oeil sur les compétences acquises de COCO. 
        </p>
      </div>

      <div id="crea">
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

#premierepartie {
  background-color: #ffa9f9;
}

.kanit-semibold {
  font-family: "Kanit", sans-serif;
  font-weight: 600;
  font-style: normal;
  font-size: 5em;
  color: blueviolet
}


.titre {
  display: flex;
  height: 350px;
  width: 100%;
  justify-content:baseline;
}

h1 {
  width: 85%;
}

#navi {
  font-size: 2em;
  text-decoration: none;
}

a {
  text-decoration: none;
}

#navi :visited {
  color: blue;
  text-decoration: underline;
}
#navi :focus {
  background: #a8e0f5;
  
}
#navi :hover {
  border-bottom: 1px solid;
  background: #ffa9f9;
}
#navi :active {
  background: #e053d7;
  color: black;
  text-decoration: underline;
  
}


.fond {
  background-image: url(/src/assets/fond.png);
  width: 100%;
  height: 100%;
}

.nav {
  display: flex;
  width: 100%;
  justify-content: space-around;
}


#cocoweb {
  position: fixed;
  width:200px ;
  height: 200px;
 
}

#souris {
  width: 150px;
}
</style>