<template>
    <div>
        <ion-header>
            <ion-toolbar>
                <ion-title>App</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content class="ion-padding">
            <ion-button id="open-modal" expand="block" @click="openModal">Open Sheet Modal</ion-button>

           
        </ion-content>
    </div>    
</template>

<script lang="ts">
import { IonButton, IonModal, IonHeader, IonContent, IonToolbar, IonTitle, IonLabel } from '@ionic/vue';
import { defineComponent } from 'vue';
import ModalContent from './ModalContent.vue';

export default defineComponent({
    components: {
        ModalContent,
        IonButton,
        IonModal,
        IonHeader,
        IonContent,
        IonToolbar,
        IonTitle,
        IonLabel,
    },
    methods: {
        openModal() {
            const modal = this.$ionic.modalController.create({
                component: ModalContent,
                swipeToClose: true,
                backdropDismiss: true,
                componentProps: {
                    // Additional props to pass to the ModalContent component
                },
            });

            modal.present();
        },
    },
});
</script>