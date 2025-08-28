<template>
  <q-page class="q-pa-lg">
    <div class="text-h4 q-mb-md">Hakkımızda</div>
    <div class="text-body1 q-mb-lg">
      <q-btn
        color="primary"
        text-color="white"
        label="SELAM"
        icon="home"
        class="q-mt-md q-mr-sm q-pt-md"
        size="xl"
      />
      <q-btn
        color="primary"
        text-color="white"
        label="SELAM"
        icon="home"
        class="q-mt-md q-mr-xl"
        size="xl"
      />

      <q-btn
        color="primary"
        text-color="white"
        icon="add"
        label="+ yeni ürün ekle"
        class="q-mt-md"
        @click="showDialog = true"
      />

      Bu örnek Quasar uygulamasında Hakkımızda sayfasıdır. İçeriği ihtiyaçlarınıza göre
      düzenleyebilirsiniz.
    </div>

    <q-dialog v-model="showDialog">
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

    <q-card flat bordered>
      <q-card-section>
        <div class="text-h6">Misyonumuz</div>
        <div class="text-body2 q-mt-sm">
          Kullanıcılarımıza modern, hızlı ve erişilebilir web uygulamaları sunmak.
        </div>
      </q-card-section>
      <q-separator />
      <q-card-section>
        <div class="text-h6">Vizyonumuz</div>
        <div class="text-body2 q-mt-sm">Teknolojiyle değer üretmek ve sürekli gelişmek.</div>
      </q-card-section>
      <q-separator />
      <q-card-section>
        <div class="text-h6">Değerlerimiz</div>
        <q-list dense bordered class="rounded-borders q-mt-sm">
          <q-item>
            <q-item-section>Şeffaflık ve güven</q-item-section>
          </q-item>
          <q-item>
            <q-item-section>Kullanıcı odaklılık</q-item-section>
          </q-item>
          <q-item>
            <q-item-section>Sürekli öğrenme ve yenilik</q-item-section>
          </q-item>
        </q-list>
      </q-card-section>
    </q-card>
  </q-page>
</template>

<script setup>
import { ref } from 'vue'
const showDialog = ref(false)
</script>

<style scoped></style>
