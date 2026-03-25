<template>
  <div id="receitas">
    <q-card clickable class="receitas-card" @click="verReceita">
      <q-card-section>
        Clique no card
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'IndexPage',
  methods: {
    verReceita() {
      this.$router.push('/receita')
    }
  }
});
</script>

<style>
#receitas {
  display: flex;
  width: 90%;
  flex-wrap: wrap;
  margin: auto;
}

.receitas-card {
  margin: 20px;
  padding: 20px;
  min-width: 20vw;
  min-height: 40vh;
  background-color: lightblue;
  cursor: pointer;
  /* flex-grow: 1; */
}
</style>
