<template>
  <div class="switch">
    <ion-label>Ou se géolocaliser :</ion-label>
    <ion-item>
      <ion-toggle
        slot="start"
        name="grape"
        color="tertiary"
        checked="false"
      ></ion-toggle>
    </ion-item>
  </div>
</template>

<script>
export default {
  name: "ToggleButton",
};
</script>

<style scoped>
.switch {
  margin-left: 3%;
  margin-top: 3%;
}
</style>