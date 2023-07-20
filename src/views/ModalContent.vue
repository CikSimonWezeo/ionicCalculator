<template>
    <IonModal></IonModal>
    <ion-page>
        <ion-content>
            <div>
                <div>
                    45,00e
                </div>
                <div>
                    <div>
                        <div @click="numberSeven()">7</div>
                        <div @click="numberEight()">8</div>
                        <div @click="numberNine()">9</div>
                    </div>
                    <div>
                        <div @click="numberFour()">4</div>
                        <div @click="numberFive()">5</div>
                        <div @click="numberSix()">6</div>
                    </div>
                    <div>
                        <div @click="numberOne()">1</div>
                        <div @click="numberTwo()">2</div>
                        <div @click="numberThree()">3</div>
                    </div>
                    <div>
                        <div @click="characterComma()">,</div>
                        <div @click="numberZero()">0</div>
                        <div @click="deleteButton()">x</div> <!-- tu bude svg -->
                    </div>
                </div>
                <div>
                    <button @click="doneButton()">Hotovo</button>
                </div>
            </div>
        </ion-content>
    </ion-page>
</template>
<script lang="ts">
import { IonPage, IonContent } from '@ionic/vue';
export default {
    components: {
        IonPage,
        IonContent,
    },
    methods: {
        numberSeven(){
            console.log("7")
        },
        numberEight() {
            console.log("8")
        },
        numberNine() {
            console.log("9")
        },
        numberFour() {
            console.log("4")
        },
        numberFive() {
            console.log("5")
        },
        numberSix() {
            console.log("6")
        },
        numberOne() {
            console.log("1")
        },
        numberTwo() {
            console.log("2")
        },
        numberThree() {
            console.log("3")
        },
        characterComma() {
            console.log(",")
        },
        numberZero() {
            console.log("0")
        },
        deleteButton() {
            console.log("x")
        },
        doneButton(){
            console.log("Hotovo")
        }
    },
}
</script>