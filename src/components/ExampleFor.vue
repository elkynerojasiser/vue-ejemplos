<template>
    <ul>
        <li v-for="pais in paises" :key="pais.codigo" v-text="pais.nombre"></li>
    </ul>
</template>
<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    name:'ExampleFor',
    data() {
        return {
            mostrar: true,
            paises : [
                {
                    "nombre" : "Colombia",
                    "codigo": "1",
                    "idioma": "Español"
                },
                {
                    "nombre" : "Usa",
                    "codigo": "2",
                    "idioma": "Inglés"
                },
                {
                    "nombre" : "Francia",
                    "codigo": "3",
                    "idioma": "Framcés"
                },
            ]
        }
        
    }
})
</script>
<style lang="scss" scoped>
</style>