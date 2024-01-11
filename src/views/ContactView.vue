
<template>
  <contactForm @soumettre="newContact"/>

</template>

<script setup>
import ContactForm from '@/components/ContactForm.vue';

const newContact = (infos) => {
  console.log(infos.name)
}
</script>