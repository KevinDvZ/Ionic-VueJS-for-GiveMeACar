<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Give me a Car</ion-title>
        <Connexion></Connexion>
      </ion-toolbar>
    </ion-header>
    <ion-content id="content" :fullscreen="true">
      <div class="placing">
        <TownPicker></TownPicker>
        <ToggleButton></ToggleButton>
        <PeriodPicker></PeriodPicker>
          <div class="carte">
        <Grid1>
            <Card></Card>
            <Card></Card>
            <Card></Card>
            <Card></Card>
            <Card></Card>
        </Grid1>
          </div>
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
import Grid1 from "@/components/Grid1.vue";
import Card from "@/components/Card.vue";
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
    Grid1,
    Card,
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
  width: 100%;
}

ion-content {
  --ion-background-color: #ecf0f7;
}

.placing {
  margin-top: 15%;
}

.carte {
  display: flex;
  width: 50%;
  margin-top: 10%;
}
</style>