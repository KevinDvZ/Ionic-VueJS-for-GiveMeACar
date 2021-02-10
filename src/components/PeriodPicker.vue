<template>
  <div class="periodPicking">
    <div class="dateText">
      <ion-label>Date de début de location :</ion-label>
    </div>

    <DatePicker></DatePicker>

    <div class="dateText">
      <ion-label>Date de fin de location :</ion-label>
    </div>

    <DatePicker></DatePicker>
  </div>
</template>

<script>
import DatePicker from "@/components/DatePicker.vue";

export default {
  name: "PeriodPicker",
  components: { DatePicker },
};
</script>

<style scoped>
.dateText {
  margin-left: 3%;
  margin-top: 3%;
  /* --padding-start: -10px; */
}
</style>