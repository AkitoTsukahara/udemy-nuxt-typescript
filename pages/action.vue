<template>
    <div>
        <div class="container">{{ first_name }} {{ last_name }}</div>
        <button @click="changeText()">{{ btnLastName }}</button>
        <button @click="backText()">{{ BtnFirstName }}</button>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'
 
export default Vue.extend({
    data: () => ({
        first_name: 'Akito',
        last_name: 'Tsukahara',
        btnLastName: 'ChangeText',
        btnFirstName: 'BackText'
    }),
    methods: {
        changeText() {
            this.first_name = 'XXXXX'
        },
        backText() {
            this.first_name = 'Akito'
        }
    }
})
</script>
 
<style></style>