<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Not a tab sub page</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Not a tab sub page</ion-title>
        </ion-toolbar>
      </ion-header>
      <div>
        <RouterLink to="/tabs/tab2"> Route to /tabs/tab2 </RouterLink>
      </div>
      <div>
        <RouterLink to="/tabs/tab2/subpage">
          Route to /tabs/tab2/subpage
        </RouterLink>
      </div>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
} from "@ionic/vue"
import { RouterLink } from "vue-router"

export default {
  name: "Tab1",
  components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,
    RouterLink,
  },
}
</script>
