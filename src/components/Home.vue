<template>
  <v-container fluid>
      <div class="pills">
          <Pil v-for="componente in nomeComponente" :key="componente.name" 
          :name="componente.name" :age="componente.age" />
      </div>
  </v-container>
</template>

<script>
import Pil from './Pil.vue'
export default {
    components: { Pil },
    data: function () {
        return {
            nomeComponente: [
                { name: 'Rafael', age: 33 },
                { name: 'Márcio', age: 40 },
                { name: 'Rafael', age: 33 }
            ]
        }
    }
}
</script>

<style>

</style>