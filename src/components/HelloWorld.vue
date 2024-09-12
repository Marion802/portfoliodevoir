<template>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Kanit:wght@600&display=swap" rel="stylesheet">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Handjet:wght@100..900&display=swap" rel="stylesheet">

<body>
      <header id="premierepartie" >
        <div class="titre">
        <h1 class="kanit-semibold"> Marion SERMANDE </h1>
        
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
      <main>
      
        <div id="present" class="handjet">
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
          <div class="modal-container">
            <div class="overlay modal-trigger"></div>
          </div>
          <div class="modal">
            <button class="close-modal modal-trigger">X</button>
            <h1>Création de CV en HTML</h1>
            <h4>Crée le <time datetime="2024-06-07"></time></h4>
            <p>Cette création fût la première, c'est un curriculum vitae qui decrit mon parcours.
              Il a été réalisé sur l'éditeur de texte Vscode et j'ai utilisée le HTML5 et le CSS3.
              La maîtrise des balises spécifiques étaient requises ainsi que la stylisation par flexbox.
              Vous pouvez retrouvez ce travail dans son intégralité par ici <a href="https://github.com/Marion802/devoircv.git"></a>
            </p>
          </div>
          <button class="modal-btn modal-trigger">Ouvrir</button>
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

#present {
  font-size: 3em;
  background-image: url(/src/assets/fond-degrade.png);
  width: 100vw;
}



.handjet {
  font-family: "Handjet", sans-serif;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
  font-variation-settings:
    "ELGR" 1,
    "ELSH" 2;
  
}

.modal-btn {
  padding: 5px 12px;
  font-size: 15px;
  margin: 100px auto;
  display: block;
  min-width: 150px;
}

.modal-container {
  position: fixed;
  top: 0;
  width: 100vw;
  height: 100vw;
}

.overlay {
  position: absolute;
  width: 100%;
  height: 100%;
  background: #333333d3;
}

.modal{
  width: 95%;
  max-width: 500px;
  min-width: 300px;
  padding: 50px;
  background: pink;
  border-radius: 5px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
}

.close-modal{
  padding: 8px 10px;
  border: none;
  border-radius: 5px;
  font-size: 18px;
  position: absolute;
  top: 10px;
  right: 10px;
  color: pink;
}

.modal h1 {
  margin-bottom: 10px;
}

.modal p{
  line-height: 1.4;
  margin-bottom: 5px;
}





#cocoweb {
  position: fixed;
  width:200px ;
  height: 200px;
 
}

#souris {
  width: 150px;
}

.uniquifier {
  font-family: "Playwrite CU";
  font-optical-sizing: auto;
  font-weight: 100;
  font-style: normal;
}




#cocoweb {
  width:150px ;
  height: 150px;
}
</style>
