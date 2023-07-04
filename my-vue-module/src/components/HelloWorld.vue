<template>
  <div>
    <p>Nombre aléatoire: {{ randomNumber }}</p>
    <button @click="generateRandomNumber">Générer un nouveau chiffre aléatoire</button>
  </div>
</template>

<script>
import getRandomNumber from '../../../index';

export default {
  data() {
    return {
      randomNumber: null,
    };
  },
  methods: {
    generateRandomNumber() {
      this.randomNumber = getRandomNumber();
    },
  },
};
</script>