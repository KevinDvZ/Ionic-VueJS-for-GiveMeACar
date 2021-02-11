<template>
  <div class="townText">
    <ion-label>Choisissez votre ville :</ion-label>
  <ion-item>
    <ion-select interface="popover">
      <ion-select-option value="nantes">Nantes</ion-select-option>
      <ion-select-option value="brest">Brest</ion-select-option>
      <ion-select-option value="morlaix">Morlaix</ion-select-option>
      <ion-select-option value="pontivy">Pontivy</ion-select-option>
      <ion-select-option value="rennes">Rennes</ion-select-option>
      <ion-select-option value="angers">Angers</ion-select-option>
      <ion-select-option value="laval">Laval</ion-select-option>
      <ion-select-option value="laRocheSurYon">La Roche-sur-Yon</ion-select-option>
    </ion-select>
  </ion-item>
  </div>
</template>

<script>
export default {
  name: "TownPicker",
};
</script>

<style scoped>

.townText {
  margin-left: 3%;
  margin-top: 3%;
}

</style>