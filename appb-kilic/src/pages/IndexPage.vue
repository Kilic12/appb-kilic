<template>
  <q-page class="flex flex-center">
    <!-- Logo -->
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-vertical.svg"
      style="width: 200px; height: 200px"
    >

    <!-- Prikaz datuma -->
    <div>
      <p>Trenutni datum: {{ currentDate }}</p>
    </div>

    <!-- Prikaz imena i prezimena -->
    <div>
      <p>Ime i prezime: {{ fullName }}</p>
    </div>
  </q-page>
</template>

<script setup>
defineOptions({
  name: 'IndexPage'
});

// Definiramo podatke za ime, prezime i datum
const fullName = "Ime Prezime";
const currentDate = new Date().toLocaleDateString();
</script>
