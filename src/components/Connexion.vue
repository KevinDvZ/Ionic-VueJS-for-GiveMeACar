<template>
  <ion-button id="ConnexionButton" color="primary">Connexion</ion-button>
  <!-- <ion-icon :icon="person"/> -->
</template>


<script>
export default {
  name: "Connexion",
};
</script>

<style scoped>
ion-button {
  --box-shadow: none;
}

#ConnexionButton {
  position: absolute;
  top: 15%;
  right: 2%;
  font-weight: bold;
  font-size: 15px;
}
</style>