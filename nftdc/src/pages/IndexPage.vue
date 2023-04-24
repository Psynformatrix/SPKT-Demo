<template>
  <q-page class="flex flex-center bg-brown-2">
    <q-card dark bordered class="inputcard bg-white my-card">
      <q-card-section>
        <div class="text-h6 text-black q-ma-md q-mb-xl">POAP Anmeldeformular</div>
        <q-input outlined class="bg-grey-4 q-ma-md q-mb-lg" v-model="text" label="Name" />
        <q-input outlined class="bg-grey-4 q-ma-md q-mb-lg" v-model="text" label="E-Mail-Adresse" />
        <q-input outlined class="bg-grey-4 q-ma-md q-mb-lg" v-model="text" label="Sparkasse" />
      </q-card-section>
      <q-card-section>
        <div>
          <q-checkbox class="text-black" v-model="right" label="Hiermit stimme ich der Verarbeitung meiner Daten zu. Bla bla bla..." />
        </div>
      </q-card-section>
      <q-card-section class="row flex-center">
        <q-btn unelevated class="q-ma-md" color="red-14" label="Eingabe bestätigen" />
        <q-btn unelevated class="q-ma-md" color="red-14" label="Pro-Button mit QR-Code" />
      </q-card-section>

      <q-separator dark inset />

      <q-card-section>
      </q-card-section>
    </q-card>
  </q-page>
</template>

<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'IndexPage',

  setup () {
    return {
      right: ref(false),
    }
  }
})

</script>

<style>
.inputcard {
  width: 30%;
}
</style>
