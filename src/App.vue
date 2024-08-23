<template>
  <ion-app>
    <ion-tabs>
      <ion-tab tab="tab1">
        <ion-content>Tab 1</ion-content>
      </ion-tab>
      <ion-tab tab="tab2">
        <ion-content>Tab 2</ion-content>
      </ion-tab>
      <ion-tab tab="tab3">
        <ion-content>Tab 3</ion-content>
      </ion-tab>

      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="tab1">
          <ion-icon :icon="triangle"></ion-icon>
          <ion-label>Tab 1</ion-label>
        </ion-tab-button>
        <ion-tab-button tab="tab2">
          <ion-icon :icon="ellipse"></ion-icon>
          <ion-label>Tab 2</ion-label>
        </ion-tab-button>
        <ion-tab-button tab="tab3">
          <ion-icon :icon="square"></ion-icon>
          <ion-label>Tab 3</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </ion-app>
</template>

<script lang="ts">
  import { IonApp, IonContent, IonLabel, IonIcon, IonTabs, IonTab, IonTabBar, IonTabButton } from '@ionic/vue';
  import { ellipse, square, triangle } from 'ionicons/icons';
  import { defineComponent } from 'vue';

  export default defineComponent({
    components: { IonApp, IonContent, IonLabel, IonIcon, IonTab, IonTabs, IonTabBar, IonTabButton },
    setup() {
      return { ellipse, square, triangle };
    },
  });
</script>