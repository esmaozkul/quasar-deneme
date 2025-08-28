<template>
  <q-page class="flex flex-center">
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-vertical.svg"
      style="width: 200px; height: 200px"
    />
    <q-dialog v-model="alert">
      <q-card>
        <q-card-section>
          <div class="text-h6">Yeni ürün ekleyebilirsiniz</div>
        </q-card-section>

        <q-card-section class="q-pt-none">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum repellendus sit voluptate
          voluptas eveniet porro. Rerum blanditiis perferendis totam, ea at omnis vel numquam
          exercitationem aut, natus minima, porro labore.
        </q-card-section>

        <q-card-actions align="right">
          <q-btn label="indirim fırsatları" color="primary" v-close-popup />
          <q-btn flat label="kapat" color="primary" v-close-popup />
        </q-card-actions>
      </q-card>
    </q-dialog>
    <q-btn
      color="primary"
      text-color="white"
      icon="add"
      label="+ yeni ürün ekle"
      class="q-mt-md"
      @click="alert = true"
    />
  </q-page>
</template>

<script setup>
import { ref } from 'vue'
const alert = ref(false)
</script>
