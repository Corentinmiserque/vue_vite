<script setup>
</script>

<template>
    <div>
      <h1>Contact</h1>
      
      <form @submit.prevent="submitForm">
        <label for="name">Nom:</label>
        <input type="text" id="name"  required>
        
        <label for="email">Email:</label>
        <input type="email" id="email" required>
        
        <label for="message">Message:</label>
        <textarea id="message"  required></textarea>
        
        <button type="submit">Envoyer</button>
      </form>
    </div>
  </template>