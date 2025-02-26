<template>
    <div class="counter">
        <h3>Counter con Option API</h3>
        <h3>{{ counter }}</h3>
        <button @click="addCounter" class="button">Incrementar</button>
    </div>
    

</template>

<script lang="ts">
// Ejemplo usando Option API
    import { defineComponent } from 'vue';

    export default defineComponent({
        name: 'CounterOption',
        components: {},
        data() {
            let counter = 0
            return {counter}
        },
        methods: {
            addCounter(){
                this.counter++
            }
        }
    })

</script>

<style scoped>
    .button{
        background-color: blueviolet;
        color: white;
        padding: 10px;
        border: 1px solid white;
    }

    .button:hover{
        background-color: white;
        color: blueviolet;
        border: 1px solid blueviolet;
    }

    .counter{
        margin: 20px;
        border: 1px solid blueviolet; 
        width: 250px;
        text-align: center;
    }
</style>