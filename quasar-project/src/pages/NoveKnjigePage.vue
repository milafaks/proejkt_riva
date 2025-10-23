<template>
  <q-page padding>
    <!-- content -->
     <h2>Nove knjige</h2>
     <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card">
      <img src="https://cdn11.bigcommerce.com/s-81ui0dgxz3/images/stencil/1280x1280/products/14725/22336/062440__22912.1743502125.jpg?c=1">

      <q-card-section>
        <div class="text-h6">Leti – dječji vodič za ptice i kako ih pronaći</div>
        <div class="text-subtitle2">by David Lindo</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://cdn.quasar.dev/img/mountains.jpg">

      <q-card-section>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">by John Doe</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem1 }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://cdn.quasar.dev/img/mountains.jpg">

      <q-card-section>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">by John Doe</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://cdn.quasar.dev/img/mountains.jpg">

      <q-card-section>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">by John Doe</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

     </div>
  </q-page>
</template>

<script>
export default {
  setup () {
    return {
      lorem: 'Širom otvori oči i uđi u čudesan svijet ptica! U dojmljivim pričama otkrij 15 prekrasnih ptica i nauči gdje ih možeš pronaći. Prati njihova nevjerojatna putovanja, uživaj u njihovoj ljepoti i saznaj kako su ta pernata bića od davnina bila nadahnuće mnogim kulturama.',
      lorem1: 'putovanja, uživaj u njihovoj ljepoti i saznaj kako su ta pernata bića od davnina bila nadahnuće mnogim kulturama.'
    }
  }
}
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px
</style>
