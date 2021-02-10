<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Give me a Car</ion-title>
        <Connexion></Connexion>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
    <div class="placing">
      <TownPicker></TownPicker>
      <ToggleButton></ToggleButton>
      <PeriodPicker></PeriodPicker>
    </div>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import {
  IonPage,
  IonHeader,
  IonTitle,
  IonToolbar,
  IonContent,
} from "@ionic/vue";
import Connexion from "@/components/Connexion.vue";
import PeriodPicker from "@/components/PeriodPicker.vue";
import TownPicker from "@/components/TownPicker.vue";
import ToggleButton from "@/components/ToggleButton.vue";
export default {
  name: "Tab798",
  components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,
    Connexion,
    TownPicker,
    ToggleButton,
    PeriodPicker,
  },
};
</script>

<style scoped>

ion-title {
  --color: #ffffff;
  margin-left: -2%;
  font-size: 22px;
  font-weight: bold;
}

ion-toolbar {
  --background: #3880ff;
    width:100%;
}

.placing {
  margin-top: 15%;
}

</style>