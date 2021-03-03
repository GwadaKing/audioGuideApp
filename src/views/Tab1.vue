<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>CHOISISSEZ UN GUIDE AUDIO</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">CHOISISSEZ VOTRE GUIDE</ion-title>
        </ion-toolbar>
      </ion-header>

      <ion-row>
        <ion-col>
            <!-- DEMO 1 BOUTONS RADIO -->
            <h4>DEMO 1 BOUTONS RADIO</h4>
            <ion-list>
              <ion-radio-group value="choixAudio">
                <ion-list-header>
                  <ion-label>Lieux à visiter</ion-label>
                </ion-list-header>

                <ion-item>
                  <ion-label>01-La cascade aux ananas</ion-label>
                  <ion-radio slot="start" value="ananas"></ion-radio>
                </ion-item>

                <ion-item>
                  <ion-label>02-La grotte aux dinosaures</ion-label>
                  <ion-radio slot="start" value="dinosaures"></ion-radio>
                </ion-item>

                <ion-item>
                  <ion-label>03-La rivière enchantée</ion-label>
                  <ion-radio slot="start" value="riviere"></ion-radio>
                </ion-item>

                <ion-item>
                  <ion-label>04-La vallée des manguiers</ion-label>
                  <ion-radio slot="start" value="mangiuers"></ion-radio>
                </ion-item>

                <ion-item>
                  <ion-label>05-Le lac aux nénuphars</ion-label>
                  <ion-radio slot="start" value="lac"></ion-radio>
                </ion-item>

              </ion-radio-group>
            </ion-list>
          </ion-col>
        </ion-row>

        <!-- DEMO 2 BOUTONS SELECT -->
        <ion-row>
          <ion-col>
            <h4>DEMO 2 BOUTONS SELECT</h4>
            <ion-list>
              <ion-list-header>
                <ion-label>
                  CHOISISSEZ UN GUIDE AUDIO
                </ion-label>
              </ion-list-header>

                <ion-item>
                  <ion-label>GUIDE AUDIO</ion-label>
                  <ion-select name="guideSelect" value="01-La cascade aux ananas" ok-text="CHOISIR" cancel-text="ANNULER" interface="alert" placeholder="01-La cascade aux ananas">
                    <ion-select-option value="01-La cascade aux ananas">01-La cascade aux ananas</ion-select-option>
                    <ion-select-option value="02-La grotte aux dinosaures">02-La grotte aux dinosaures</ion-select-option>
                    <ion-select-option value="03-La rivière enchantée">03-La rivière enchantée</ion-select-option>
                    <ion-select-option value="04-La vallée des manguiers">04-La vallée des manguiers</ion-select-option>
                    <ion-select-option value="05-Le lac aux nénuphars">05-Le lac aux nénuphars</ion-select-option>
                  </ion-select>
                </ion-item>
            </ion-list>
          </ion-col>
        </ion-row>

        <!-- DEMO 3 SLIDER RANGE -->
        <ion-row>
          <ion-col>
            <h4>DEMO 3 SLIDER RANGE</h4>
            <ion-list>

              <ion-item>
                <ion-range min="1" max="100" pin="true" color="secondary">
                  <ion-label slot="start">1</ion-label>
                  <ion-label slot="end">100</ion-label>
                </ion-range>
              </ion-item>
            </ion-list>
          </ion-col>
        </ion-row>


    </ion-content>
  </ion-page>
</template>

<script>
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';

export default  {
  name: 'Tab1',
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage }
}
</script>