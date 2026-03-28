<template>
  <div class="page">
    <div class="pageCase">
      <div class="pageCaseLeft">
        <q-img
          src="https://media.istockphoto.com/id/1326149453/pt/foto/dark-chocolate-cake-slice.webp?s=1024x1024&w=is&k=20&c=Z30KsJMyK4nhpEnpFCNFHnT36ICSr_pMIfZ-XY-n-qk="
          class="rounded-borders">
          <div class="legenda absolute-bottom text-subtitle1 text-center">
            Bolo de chocolate
          </div>
        </q-img>
        Por João
        <div class="q-pa-md">
          INGREDIENTES:
          <div class="ingredients q-gutter-sm">
            <q-checkbox v-model="selection" val="teal" label="3 Ovos" color="teal" />
            <q-checkbox v-model="selection" val="orange" label="Uma Pitada de Sal" color="teal" />
            <q-checkbox v-model="selection" val="red" label="Red" color="teal" />
            <q-checkbox v-model="selection" val="cyan" label="Cyan" color="teal" />
          </div>

          <!-- <div class="q-px-sm">
            The model data: <strong>{{ selection }}</strong>
          </div> -->
        </div>
      </div>
      <div class="pageCaseRight">
        coluna direita
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    return {
      selection: ref(['teal', 'red'])
    }
  }
}
</script>

<style>
.page {
  background-color: lightblue;
}

.pageCase {
  display: flex;
  width: 1200px;
  margin: auto;
  padding: 20px 0;
  background-color: lightgreen;
  gap: 10px;
}

.pageCaseLeft {
  flex-grow: 3;
  background-color: lightyellow;
}

.pageCaseRight {
  flex-grow: 1;
  background-color: lightcoral;
}

.legenda {
  font-size: 2rem;
  font-weight: bold;
  text-transform: uppercase;
}

.ingredients {
  display: flex;
  flex-direction: column;
}
</style>