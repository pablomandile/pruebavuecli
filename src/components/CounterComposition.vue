<template>
    <div class="counter">
        <h3>Counter con Composition API</h3>
        <h3>{{ counter }}</h3>
        <button @click="addCounter" class="button">Incrementar</button>
    </div>
    
</template>

<!-- ************ Script sin usar Setup -->

<!-- <script lang="ts">
    import { defineComponent, ref } from 'vue'

    export default defineComponent ({
        name: 'CounterComposition',
        components: {},
        setup() {
            let counter = ref(0)
            const addCounter = () => {
                counter.value++
            }
            return { counter, addCounter }
        }
    })

</script> -->

<!-- ************ Script usando Setup ahorramos código -->

<script lang="ts" setup>
    import { ref, Ref } from 'vue'

    let counter:Ref = ref(0)    // Ref se usa para tipar
    const addCounter = () => {
        counter.value++
    }


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