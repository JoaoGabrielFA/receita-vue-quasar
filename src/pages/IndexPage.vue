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
    width: 100%;
    flex-wrap: wrap;
  }

  #receitas-card{
    margin: 20px;
    padding: 20px;
    min-width: 20vw;
    min-height: 40vh;
    background-color: lightblue;
  }
</style>
