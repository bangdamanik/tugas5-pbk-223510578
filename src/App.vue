<template>
  <div class="q-pa-md q-gutter-sm flex-between aa">
    <div class="left">
      <q-avatar class="profile">
        <q-icon name="account_circle" size="45px" />
      </q-avatar>
    </div>
    <div class="right">
      <q-btn flat style="color: #001499cc" label="Kontak" />
      <q-btn flat style="color: #001499cc" label="Pengaturan" />
      <q-btn style="background: #001499cc; color: white" label="Login" />
    </div>
  </div>

  <div class="q-pa-md">
    <q-carousel
      v-model="slide"
      swipeable
      animated
      navigation-position="bottom"
      navigation
      padding
      height="200px"
      class="bg-indigo-9 text-white rounded-borders"
    >
      <q-carousel-slide name="style" class="column no-wrap flex-center">
        <q-icon name="shopping_cart" size="56px" />
        <div class="q-mt-md text-center">
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="layers" class="column no-wrap flex-center">
        <q-icon name="local_mall" size="56px" />
        <div class="q-mt-md text-center">
        </div>
      </q-carousel-slide>
    </q-carousel>
  </div>

  <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card" flat bordered>
      <q-img
        src="https://static.promediateknologi.id/crop/0x0:0x0/0x0/webp/photo/p2/01/2023/04/28/New-Xpander-Cross-Mudik-483028941.jpg"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 180.000.000.00</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Xpander</div>
        <div class="text-caption text-grey">
          Km 12.000, bebas banjir
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="https://cdn.quicksell.co/-MjvT0UfXEns6okX2V1C/products/-NPw_iwV4Ea_YfFgUQFQ.jpg"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 390.000.000.00</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Pajero Dakar 4x2</div>
        <div class="text-caption text-grey">
          Km 12.000, bebas banjir
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="https://asset.kompas.com/crops/pqNZKu-rk4RixzgXJOhwe7sEC6g=/0x0:6000x4000/1200x800/data/photo/2022/01/13/61e03fda79c68.jpg"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 380.000.000.00</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Fortuner Gr Sport</div>
        <div class="text-caption text-grey">
          Km 12.000, bebas banjir
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="https://cdn.quicksell.co/-My6FfBpPDhAjmjgfvus/products/-NGB1BnIpzFOj2AMVklA.jpg"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 340.000.000.00</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Innova V 2.0</div>
        <div class="text-caption text-grey">
          Km 12.000, bebas banjir
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>
  </div>

    <footer class="q-pa-md text-center bg-indigo-10 text-white">
      <div class="text-caption">Tapung | Tapung Jaya Mobilindo</div>
    </footer>


</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref('style'),
      expanded: ref(false),
      lorem: 'Harga cari aja disini bosku, barang ready selalu'
    }
  }
}
</script>

<style scoped>
.flex-between {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #e3e3e3;
  padding: 1rem 3rem;
}


.left {
  display: flex;
  align-items: center;
}

.right {
  display: flex;
  align-items: center;
}

.my-card {
  width: 100%;
  max-width: 350px;
}

.same-size-image {
  width: 100%;
  height: 400px;
  object-fit: cover;
}

.aa{
  max-width: 100%;
}


</style>