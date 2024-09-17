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
            <div class="nav handjet">
              <img src="/src/assets/souris.png" alt="une souris d'ordinateur rose" id="souris">
              <nav class="kanit-semibold" id="navi">
              <ul>
                <li> <a href="#present">Présentation</a></li>
                <li> <a href="#font">Création</a></li>
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
          </main>
    </body>
    
</template>    


<script>

</script>


<style scoped>



#premierepartie {
  background-color: #ffa9f9;
  margin: 0;
  padding: 0;
}

body { 
    margin: 0;
    padding: 0;
}

.kanit-semibold {
  font-family: "Kanit", sans-serif;
  font-weight: 600;
  font-style: normal;
  font-size: 5em;
  color: blueviolet
}


.titre {
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
    color: blueviolet;
  font-size: 3em;
  background-image: url(/src/assets/fond-degrade.png);
  width: 100%;
  margin: 0;
  padding: 0;
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






#cocoweb {
  position: fixed;
  top: 0;
  right: 0;
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
  width:250px ;
  height: 250px;
}



</style>


