<template>
<h2>Date de début de location:</h2>
  <datepicker></datepicker>
  <h2>Date de fin de location:</h2>
  <datepicker></datepicker>

</template>

<script>
import datepicker from '@/components/date-picker.vue'

export default {
  name: "periode-picker",
  components: {datepicker}

}
</script>

<style scoped>

</style>