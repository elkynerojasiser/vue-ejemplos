<template>
    <h1>Mi formulario</h1>
    <br>
    <label for="">Nombre</label>
    <br>
    <input v-model="nombre" type="text" >
    <br>
    <button @click="mostrarNombre">Ver dato</button>
    <button @click="ocultarNombre">Ocultar dato</button>

    <br><br>
    <div>
        <h3 v-show="mostrar">{{ nombre }}</h3>
    </div>

    <img :src="require(`@/assets/${imagen}`)" alt="" width="200">
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    name:'ExampleModel',
    data() {
        return {
            mostrar:false,
            nombre:"Pepito",
            imagen:"ejemplo.jpg"
        }
    },
    methods: {
        mostrarNombre() {
            this.mostrar = true
        },
        ocultarNombre() {
            this.mostrar = false
        }

    }
})
</script>

<style lang="scss">
</style>