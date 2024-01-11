<template>
  <div>
    <h1>Contact</h1>
    
    <form @submit.prevent="submitForm">
      <label for="name">Nom:</label>
      <input type="text" v-model="newContact.name" id="name" >
      
      <label for="email">Email:</label>
      <input type="email" id="email"v-model="newContact.email" >
      
      
      <button type="submit">Envoyer</button>
    </form>
  </div>
</template>

<script setup>
//import
import { ref } from 'vue';


//code
const newContact = ref({
  name: "",
  email:""
})
const emit = defineEmits(['soumettre'])

const submitForm = () => {
  alert('test');
  emit('soumettre'), newContact.value
};

</script>
