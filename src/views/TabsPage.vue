<template>
  <ion-page>
    <ion-tabs>
      <ion-router-outlet></ion-router-outlet>
      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="tab1" href="/trends">
          <ion-icon aria-hidden="true" :icon="flameOutline" />
          <ion-label>Trend</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="tab2" href="/meme">
          <ion-icon aria-hidden="true" :icon="diceOutline" />
          <ion-label>Meme</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="tab3" href="/category">
          <ion-icon aria-hidden="true" :icon="appsOutline" />
          <ion-label>Categorie</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>

<script setup lang="ts">
import { IonTabBar, IonTabButton, IonTabs, IonLabel, IonIcon, IonPage, IonRouterOutlet } from '@ionic/vue';
import { flameOutline, appsOutline, diceOutline } from 'ionicons/icons';
</script>
