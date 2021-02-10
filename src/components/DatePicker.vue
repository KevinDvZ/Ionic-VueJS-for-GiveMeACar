<template>
  <!-- Mettre un ion-button?????????? -->
  <div class="datePicking">
    <ion-button shape="round" fill="solid">
      <ion-datetime
        displayFormat="D/M/YYYY"
        pickerFormat="D MM YYYY"
        value="02 10 2021"
        placeholder="Quel jour?"
      ></ion-datetime>
    </ion-button>
  </div>
  <!-- Mettre un ion-button?????????? -->
</template>

<script>
export default {
  name: "DatePicker",
};
</script>

<style scoped>

.datePicking {
  margin-top: 2%;
}

ion-button {
  margin-left: 5%;
  font-size: 20px;
}

ion-datetime::part(text) {
  display: flex;
  align-items: center;
  margin-left: -5%;
}

</style>