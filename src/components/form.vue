<template>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Handjet:wght@100..900&display=swap" rel="stylesheet">
    


    <div class="form handjet">
<form @submit.prevent="sendEmail" id="formulaire">
            <h2>Contactez Coco</h2>
            <div>
              <label for="first-name">Prénom</label>
              <input type="text" name="first-name" id="first-name" v-model="formData.name">
            </div>
            
            <div>
              <label for="last-name" >Nom</label>
                <input type="text" name="last-name" id="last-name" v-model="formData.lastName">
            </div>
            
            <div>
              <label for="object" >Objet</label>
                <input type="text" name="object" id="object" v-model="formData.object">
            </div>
            
            <div>
              <label for="message" >Commentaire</label>
              <textarea id="message" name="message" rows="4"  v-model="formData.message"></textarea>
            
            </div>
            <button type="submit" value="send"> Envoyer </button>
          </form>
        </div>
</template>



<script setup>
import emailjs from '@emailjs/browser';
import { ref} from 'vue';
const formData = ref ({
    name : '',
    lastName : '',
    object : '',
    message : '',
});
const sendEmail = async () => {
    try{
        const templateParams = {
            from_name : formData.value.name,
            from_last_name: formData.value.lastName,
            from_object: formData.value.object,
            from_message: formData.value.message
        }
        console.log('templateParams:', templateParams)

            await emailjs.send('service_oudfzfc','template_xy4wbde', templateParams, 'M6tb_IXBNXDqsZe9m')
            alert ('Email sent successfully')
            formData.value.name=''
            formData.value.lastName=''
            formData.value.object=''
            formData.value.message=''

    }catch (error) {
        console.error(error)
        alert('Error sending email. Please try again')
    }
}

</script>




<style scoped>

#formulaire {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: auto 0;
    border: 1px solid purple;
    padding: 20px;
    right: 50%;
    left: 50%;
    background: pink;
}

input {
    margin-bottom: 20px;
}

textarea {
    font-size: 1em;
}

.handjet {
  color : blueviolet;
  font-family: "Handjet", sans-serif;
  font-size: 2em;
  font-weight: 400;
  font-style: normal;
  font-variation-settings:
    "ELGR" 1,
    "ELSH" 2;
}


button{
    color: blueviolet;
    background-color: aquamarine;
    cursor: pointer;
}
</style>