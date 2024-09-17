
<template>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Handjet:wght@100..900&display=swap" rel="stylesheet">
    
   
   
   
  <premierepartie></premierepartie>
   
   
   
  <div id="font" class="handjet">
    <div id="cv">
      <h2>CV en html</h2>
      <button @click="showModal=true"><img src="./assets/hautcv.png" alt="aperçu d'un cv" class="hautcvv"></button>
      <Modal v-if="showModal" @close="showModal=false" class="modal">
        <h3>Création de CV en HTML</h3>
            <h4>Crée le <time datetime="2024-07-06"> 06 Juillet 2024</time></h4>
            <a target="blank" href="./assets/hautcv.png"><img src="./assets/hautcv.png" alt="photo cv" class="photocv"></a>
            <img src="./assets/middlecv.png" alt="photo cv" class="photocv">
            <img src="./assets/bascv.png" alt="photo cv" class="photocv">
              <p>Cette création fût la première, c'est un curriculum vitae qui decrit mon parcours.
              Il a été réalisé sur l'éditeur de texte Vscode et j'ai utilisée le HTML5 et le CSS3.
              La maîtrise des balises spécifiques étaient requises ainsi que la stylisation par flexbox.
              Vous pouvez retrouvez ce travail dans son intégralité <a target="blank" href="https://github.com/Marion802/devoircv.git">ICI</a>
              </p>
      </Modal>
    </div>

    <div id="cahierdescharges" class="handjet">
          <h2>Cahier des charges</h2>
            <p>Il s’agit d’un document que l’on utilise 
              dans le cadre du développement d’un projet. Sa rédaction suit en général des normes assez fixes.
              Il sert à définir la finalité d’un projet, les étapes pour sa réalisation et les éléments 
              nécessaires pour le mener à bien. On peut aussi le considéré comme les termes 
              d'un contrat entre l'entreprise et le client.</p>
            <button @click="showCdc=true"><img src="./assets/couverturecdc.png" alt="photo couverture" class="photocdc"></button>
            <Cdc v-if="showCdc" @close="showCdc=false" class="modal">
              <h3>Création d'un cahier des charges</h3>
              <p>Créer le <time datetime="2024-07-20">20 Juillet 2024</time></p>
              <img src="./assets/lasock.png" alt="photo document" class="photosock">
              <img src="./assets/lasocke.png" alt="photo document" class="photosock">
              <img src="./assets/lasocket.png" alt="photo document" class="photosock">
              <p>Ici nous retrouvons un cahier des charges qui a été réalisé par nos soin pour l'entreprise
                La Socketterie qui souhaité revoir son site web qui était jusque là un site vitrine pour 
                en faire un site e-commerce. Si vous quittez ces aperçut et allez voir de plus près mon travail
                vous découvrirez la structure d'un projet de A à Z avec tout les composants de ce dernier.
                Une présentation globale de l'entreprise et des objectifs visés. Au niveau de l'ergonomie une 
                charte graphique pour le respect des couleurs ainsi qu'une représentation de l'architecture du site.
                Le cahier des charges contient les spécificités des demandes du clients avec des exemples concrets.
                Pour finir, un devis et un agenda de planning a respecter.</p>
                <p><a target="blank"  href="./assets/lasocketterie_240912_021209(1).pdf">Mon cahier des charges</a></p>
            </Cdc>
    </div>
    
        


        <div id="espacecomment" class="handjet">
          <h3>Dynamiser un espace commentaire</h3>
            <p>Ceci est un exemple de ce que nous pouvons realiser avec JavaScript</p>
              <button @click="showComment=true"><img src="./assets/commentenvoit.png" alt="photo document" class="commentaire"></button>
              <Comment v-if="showComment" @close="showComment=false" class="modal">
                <h3>Dynamiser un espace commentaire</h3>
                  <p>Créer le <time datetime="2024-08-27">27 Aout 2024</time></p>
                  <img src="./assets/comment.png" alt="photo document" class="escom">
                  <img src="./assets/commentenvoit.png" alt="photo document" class="escom">
                  <p>JavaScript est un language de programmation avec lequel 
                    nous pouvons réalisé de grand projet. Ces photos représente 
                    un exemple d'espace commentaire ou nous avons pu realisé des messages d'erreurs
                    si un champs est manquant ainsi que l'envoie du commentaire dans la liste présente.
                    Vous pouvez découvrir ce travail <a target="blank"   href="https://github.com/Marion802/devoircommentaire.git">ICI</a>
                  </p>
              </Comment>
          </div>
  </div>



  <formulaire></formulaire>


  <pied></pied>



</template>




<script setup >
import { ref , defineProps} from 'vue';
import Modal from '@/components/HelloWorld.vue'
let showModal = ref(false)
defineComponent({Modal})

import Cdc from '@/components/cdc.vue'
let showCdc =ref(false)
defineComponent({Cdc})

import Comment from '@/components/comment.vue'
let showComment = ref(false)
defineComponent({Comment})

import premierepartie from '@/components/corps.vue'

import pied from '@/components/footer.vue';

import formulaire from '@/components/form.vue';
import { defineComponent } from 'vue';

let font = 'mon-ancrage'



</script>


<style scoped>

  #espacecomment {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  #cahierdescharges {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  #cv {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  #font {
    margin: 0px;
    padding: 0px;
    background-color: #ffa9f9;
    font-size: 1.5em;
  }

  .handjet {
    color: blue;
  font-family: "Handjet", sans-serif;
  font-weight: 400;
  font-style: normal;
  font-variation-settings:
    "ELGR" 1,
    "ELSH" 2;
  
}
 .hautcvv {
  height: 400px;
  width: 400px;
  cursor: pointer;
 }
 .hautcvv:hover{
  box-shadow: 10px 10px 10px rgba(100, 97, 97, 0.2);
 }

 .photocv {
  height: 300px;
  width: 300px;
 }

 .photocdc {
  height: 300px;
  cursor: pointer;
 }

.photocdc:hover {
  box-shadow: 10px 10px 10px rgba(100, 97, 97, 0.2);
}


 .photosock {
  height: 250px;
  width: 300px;
 }

 .commentaire {
  height:300px ;
  cursor: pointer;
 }
 .commentaire:hover {
  box-shadow: 10px 10px 10px rgba(100, 97, 97, 0.2);
 }
 


 .escom {
  height: 300px;
  width: 450px;
 }
</style>


