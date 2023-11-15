<template>
  <main class="main">
    <div class="container">
      <div class="header__top">
        <div class="header__top-content">
          <h1 class="header__top-h1">spacody - webamooz</h1>
          <p class="header__top-p">be professional</p>
        </div>
        Hi I amGere.
      </div>
      
    </div>
  </main>
</template>

<script>
import { mapGetters } from 'vuex'
import SwiperSlider from '../components/SwiperSlider'
export default {
  name: 'Test',

  metaInfo: {
    titleTemplate: null
  },

  components: {
    SwiperSlider
  },

  data: () => ({
    slides: [
      { img: require('@/assets/img/slideshow/1.png') },
      { img: require('@/assets/img/slideshow/2.png') },
      { img: require('@/assets/img/slideshow/3.png') },
      { img: require('@/assets/img/slideshow/4.png') }
    ],
    slideShowIndex: 0,
    sliderInterval: null,
    progressWidth: 0
  }),

  computed: {
    ...mapGetters('products', ['products'])
  },

  methods: {
    move(n) {
      if (this.slides.length <= this.slideShowIndex + n) {
        this.slideShowIndex = 0
      } else if (this.slideShowIndex + n < 0) {
        this.slideShowIndex = this.slides.length - 1
      } else {
        this.slideShowIndex += n
      }
    },
    formattedPrice(price) {
      return new Intl.NumberFormat('en', {
        style: 'currency',
        currency: 'USD'
      }).format(price)
    }
  },

  created() {
    this.$store.dispatch('products/getProducts', { text: 'dfjghkdfhgdrigh' })
    this.sliderInterval = setInterval(() => {
      if (this.progressWidth >= 100) {
        this.progressWidth = 0
        this.move(1)
      } else {
        this.progressWidth++
      }
    }, 15)
  },

  unmounted() {
    clearInterval(this.sliderInterval)
  }
}
</script>
