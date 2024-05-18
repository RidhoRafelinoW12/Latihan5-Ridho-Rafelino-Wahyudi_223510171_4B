<template>
  <q-layout view="hHh lpR fFf">
    <q-header :class="headerClass" elevated height-hint="98">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="toggleLeftDrawer" />

        <q-toolbar-title>
          <q-avatar>
            <img src="./assets/pp12.jpg">
          </q-avatar>
          Avocado09Store
        </q-toolbar-title>

        <q-btn dense flat round icon="shopping_cart" @click="toggleRightDrawer" />
      </q-toolbar>

      <q-tabs align="left">
        <q-route-tab to="/home" label="Home" />
        <q-route-tab to="/about-us" label="About Us" />
        <q-route-tab to="/products" label="Products" />
        <q-route-tab to="/contact" label="Contact" />
      </q-tabs>
    </q-header>

    <q-drawer show-if-above v-model="leftDrawerOpen" side="left" bordered>
      <q-list>
        <q-item-label header>Kategori</q-item-label>
        <q-item clickable v-ripple>
          <q-item-section>Hoodie</q-item-section>
        </q-item>
        <q-item clickable v-ripple>
          <q-item-section>Crewneck</q-item-section>
        </q-item>
        <q-item clickable v-ripple>
          <q-item-section>Celana</q-item-section>
        </q-item>
        <q-item clickable v-ripple>
          <q-item-section>Kemeja</q-item-section>
        </q-item>
        <q-item clickable v-ripple>
          <q-item-section>Kaos</q-item-section>
        </q-item>
      </q-list>
    </q-drawer>

    <q-drawer show-if-above v-model="rightDrawerOpen" side="right" bordered>
      <q-list>
        <q-item-label header>Shopping Cart</q-item-label>
        <q-item>
          <q-item-section>Hoodie "SukunaxFullFingers"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp5.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Celana "Doodle"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp7.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodiex"Skeleton"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp9.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodie "Cigerrates After Sex"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp1.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodie "Avenged Sevenfold"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp2.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Crewneck "Sukuna"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp3.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Crewneck "Sukuna(v2)"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp4.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Crewneck "Sukuna(v3)"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp6.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodie "Totoro"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp8.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodie "White Black left Skeleton"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp10.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodie "Cry Ending"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp11.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodie "Nirvana"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp13.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodie "Avenged Sevenfold(v2)"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp14.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodie "Mahoraga Summon"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp15.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Hoodie "Arctic Monkeys"</q-item-section>
          <q-item-section side>
            <q-carousel-slide :name="1" img-src="./assets/pp16.jpg" />
            <q-btn round dense icon="remove_circle" />
            <q-btn round dense icon="add_circle" />
          </q-item-section>
        </q-item>
        <q-separator />
        <q-item>
          <q-item-section>Total</q-item-section>
          <q-item-section side>$120.00</q-item-section>
        </q-item>
        <q-btn color="primary" label="Checkout" class="full-width q-ma-sm" />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
      <!-- Carousel Section -->
      <div class="q-pa-md">
        <q-carousel
          swipeable
          animated
          v-model="slide"
          :autoplay="autoplay"
          ref="carousel"
          infinite
          @slide="onSlideChange"
        >
          <q-carousel-slide :name="1" img-src="./assets/pp1.jpg" />
          <q-carousel-slide :name="2" img-src="./assets/pp2.jpg" />
          <q-carousel-slide :name="3" img-src="./assets/pp3.jpg" />
          <q-carousel-slide :name="4" img-src="./assets/pp4.jpg" />
          <q-carousel-slide :name="5" img-src="./assets/pp5.jpg" />
          <q-carousel-slide :name="6" img-src="./assets/pp6.jpg" />
          <q-carousel-slide :name="7" img-src="./assets/pp7.jpg" />
          <q-carousel-slide :name="8" img-src="./assets/pp8.jpg" />
          <q-carousel-slide :name="9" img-src="./assets/pp9.jpg" />
          <q-carousel-slide :name="10" img-src="./assets/pp10.jpg" />
          <q-carousel-slide :name="11" img-src="./assets/pp11.jpg" />
          <q-carousel-slide :name="13" img-src="./assets/pp13.jpg" />
          <q-carousel-slide :name="14" img-src="./assets/pp14.jpg" />
          <q-carousel-slide :name="15" img-src="./assets/pp15.jpg" />
          <q-carousel-slide :name="16" img-src="./assets/pp16.jpg" />

          <template v-slot:control>
            <q-carousel-control
              position="top-right"
              :offset="[18, 18]"
              class="text-white rounded-borders"
              style="background: rgba(0, 0, 0, .3); padding: 4px 8px;"
            >
              <q-toggle dense dark color="orange" v-model="autoplay" label="Auto Play" />
            </q-carousel-control>

            <q-carousel-control
              position="bottom-right"
              :offset="[18, 18]"
              class="q-gutter-xs"
            >
              <q-btn
                push round dense color="orange" text-color="black" icon="arrow_left"
                @click="$refs.carousel.previous()"
              />
              <q-btn
                push round dense color="orange" text-color="black" icon="arrow_right"
                @click="$refs.carousel.next()"
              />
            </q-carousel-control>
          </template>
        </q-carousel>
        <div class="text-center q-mt-md">
          Slide {{ slide }} of {{ totalSlides }}
        </div>

        <!-- Add the single card here -->
        <div class="q-pa-md row items-start q-gutter-md">
          <q-card
            class="my-card text-white"
            style="background: radial-gradient(circle, #35a2ff 50%, #000000 100%)"
          >
            <q-card-section>
              <div class="text-h6">Selamat Datang di Avocado09Store!!!</div>
              <div class="text-subtitle2">saya Ridho rafelino Wahyudi mengucapkan selamat datang dan berterima kasih atas calon customer 
              yang datang untuk melihat produk-produk yang kami buat. Mungkin Produk-produk yang kami tawarkan masih terbilang jauh, 
              namun kami "Avocado09Store" yakin kami bisa meraih ke tempat yang lebih baik lagi, semua berkat komen,kritik, serta saran 
              dari calon-calon customer kesayangan kami, Sekian Terima Kasih!!!</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
              {{ lorem }}
            </q-card-section>
          </q-card>
        </div>
      </div>
    </q-page-container>

    <q-footer :class="footerClass" elevated>
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="./assets/pp12.jpg">
          </q-avatar>
          Avocado09Store
        </q-toolbar-title>
        <q-toggle dense dark color="orange" v-model="isDarkTheme" label="Dark Theme" @change="toggleTheme" />
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script>
import { ref, computed } from 'vue'

export default {
  setup () {
    const leftDrawerOpen = ref(false)
    const rightDrawerOpen = ref(false)
    const isDarkTheme = ref(false)
    const slide = ref(1)
    const autoplay = ref(false)
    const totalSlides = ref(16)

    const headerClass = computed(() => isDarkTheme.value ? 'bg-dark text-white' : 'bg-primary text-white')
    const footerClass = computed(() => isDarkTheme.value ? 'bg-dark text-white' : 'bg-grey-8 text-white')

    const toggleLeftDrawer = () => {
      leftDrawerOpen.value = !leftDrawerOpen.value
    }

    const toggleRightDrawer = () => {
      rightDrawerOpen.value = !rightDrawerOpen.value
    }

    const toggleTheme = () => {
      isDarkTheme.value = !isDarkTheme.value
    }

    const onSlideChange = (newSlide) => {
      slide.value = newSlide
    }

    return {
      leftDrawerOpen,
      rightDrawerOpen,
      isDarkTheme,
      headerClass,
      footerClass,
      toggleLeftDrawer,
      toggleRightDrawer,
      toggleTheme,
      slide,
      autoplay,
      totalSlides,
      onSlideChange
    }
  }
}
</script>

<style>
.bg-dark {
  background-color: #1d1d1d !important;
}
.text-white {
  color: white !important;
}
.full-width {
  width: 100%;
}
.my-card {
  width: 100%;
  max-width: 250px;
}
</style>