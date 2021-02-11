<template>
  <div class="townText">
     <ion-label>Choisissez votre ville :</ion-label>
   <ion-item>
    <ion-select interface="popover"
    placeholder="Choisissez une agence"
    :value="selectedOption"
    @ionChange="selectedOption= $event.target.value">
      <ion-select-option
      class="ion-text-capitalize"
      v-for="(agence, idAgence) in listeAgences"
      :key="idAgence"
      :value="agence.ville"
      > {{agence.ville}} </ion-select-option>
    </ion-select>
  </ion-item>
  </div>

</template>

<script>
export default {
  name: "TownPicker",
  data: function() {
return {
    listeAgences: [],
  };
},
  methods : {
    fetchData () {
      fetch(`http://warm-cove-08783.herokuapp.com/agences`)
          .then(res => res.json())
          .then(post =>  this.remplirTableau(post))
    },
    remplirTableau (item) {
      this.listeAgences = item;

    },
    log(item){
      console.log(item)
    }
  },
  created(){
    this.fetchData();

  }
};
</script>

<style scoped>

.townText {
  margin-left: 3%;
  margin-top: 3%;
}

</style>