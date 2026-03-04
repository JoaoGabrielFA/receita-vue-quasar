<template>
  <div id="receitas">
    <q-card id="receitas-card">
      receita card
    </q-card>
    <q-card id="receitas-card">
      receita card
    </q-card>
    <q-card id="receitas-card">
      receita card
    </q-card>
    <q-card id="receitas-card">
      receita card
    </q-card>
    <q-card id="receitas-card">
      receita card
    </q-card>
  </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'IndexPage'
});
</script>

<style>
  #receitas {
    display: flex;
    width: 90%;
    flex-wrap: wrap;
    margin: auto;
  }

  #receitas-card{
    margin: 20px;
    padding: 20px;
    min-width: 20vw;
    min-height: 40vh;
    background-color: lightblue;
    /* flex-grow: 1; */
  }
</style>
