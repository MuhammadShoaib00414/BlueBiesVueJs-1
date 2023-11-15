<template>
  <section class="about-holder py-5 d-none d-md-block border-b-r-light">
    <div class="container pb-5 pt-4">

      <div class="text-center">
        <h1 class="mt-4">الفرص التجارية والعملاءالمرتقبين الآن أقرب!</h1>
        <ul class="list-unstyled list-inline my-4">
          <li class="list-inline-item animate-box right-in px-2"><a href="about.html" title="تعرف علي بلوبيز"
              class="text-primary"><i class="icofont-play-alt-1 ml-1"></i> تعرف علي بلوبيز</a></li>
          <li class="list-inline-item animate-box left-in px-2"><a href="#ordersSec" class="smooth-a"
              title="عرض الطلبات الجديدة">عرض الطلبات الجديدة</a></li>
        </ul>
        <div class="animate-box my-5">
          <img src="images/home-img.png" alt="image" class="home-img">
        </div>
      </div>

      <p class="m-0">كيف يعمل بلوبيز؟</p>
      <div class="row mb-5">
        <div class="col-md-4">
          <h2 class="hover-primary">إنشئ ملف شركتك</h2>
        </div>
        <div class="col-md-4">
          <h2 class="hover-primary">تابع الطلبات الجديدة</h2>
        </div>
        <div class="col-md-4">
          <h2 class="hover-primary">المعلمين</h2>
        </div>
      </div>

      <div class="animate-box pt-4" id="aboutSec">
        <div class="owl-carousel">

          <div class="item p-1">
            <div class="row">

              <div class="col-5 col-lg-6 pr-5">
                <h2 class="mt-5 pt-4 mb-3">ملئ بياناتك</h2>
                <h5>كتابة كافة تفاصيل ملف شركتك كالأسم, طرق التواصل, الصناعة المتخصصة فيها.</h5>
                <a href="register.html" class="btn btn-primary mt-3" title="اشترك الان">اشترك الان</a>
              </div>

              <div class="col-7 col-lg-6">
                <div class="card m-0 animate-box">
                  <div class="card-body">
                    <i class="fa fa-user-plus"></i>
                    <h4>إشتراك جديد</h4>
                    <form method="post" action="#">
                      <div class="row">
                        <div class="col-6">
                          <label class="text-muted">اسم المؤسسة
                            <input type="text" class="border border-light mt-1">
                          </label>
                        </div>
                        <div class="col-6">
                          <label class="text-muted">البريد الالكتروني
                            <input type="email" class="border border-light mt-1">
                          </label>
                        </div>
                        <div class="col-6">
                          <label class="text-muted">عنوان شركتك
                            <input type="text" class="border border-light mt-1">
                          </label>
                        </div>
                        <div class="col-6">
                          <label class="text-muted">رقم التواصل
                            <input type="tel" class="border border-light mt-1">
                          </label>
                        </div>
                        <div class="col-6">
                          <label class="text-muted">كلمة المرور
                            <input type="pass" class="border border-light mt-1">
                          </label>
                        </div>
                        <div class="col-6">
                          <label class="text-muted">تأكيد كلمة المرور
                            <input type="pass" class="border border-light mt-1">
                          </label>
                        </div>
                      </div>
                      <button type="submit" class="btn btn-primary">اشترك</button>
                    </form>
                  </div>
                </div>
              </div>

            </div>
          </div>

          <div class="item p-1">
            <div class="row">

              <div class="col-5 col-lg-6 pr-5">
                <h2 class="mt-5 pt-4 mb-3">ملئ بياناتك</h2>
                <h5>كتابة كافة تفاصيل ملف شركتك كالأسم, طرق التواصل, الصناعة المتخصصة فيها.</h5>
                <a href="register.html" class="btn btn-primary mt-3" title="اشترك الان">اشترك الان</a>
              </div>

              <div class="col-7 col-lg-6">
                <div class="card m-0 animate-box">
                  <div class="card-body">
                    <i class="fa fa-users"></i>
                    <h4>تسجيل الدخول</h4>
                    <form method="post" action="#">
                      <label class="text-muted d-block">اسم المؤسسة
                        <input type="text" class="border border-light mt-1">
                      </label>
                      <label class="text-muted d-block">كلمة المرور
                        <input type="text" class="border border-light mt-1">
                      </label>
                      <p><a href="#" title=".." class="text-primary">هل نسيت كلمة المرور؟</a></p>
                      <button type="submit" class="btn btn-primary">تسجيل الدخول</button>
                    </form>
                  </div>
                </div>
              </div>

            </div>
          </div>

        </div>
      </div>
    </div>
  </section>
  <section class="orders-holder pt-md-5 pb-5 bg-light border-b-l-white" id="ordersSec">
    <orderRecived></orderRecived>
  </section>
  <section class="partners-holder py-5 d-none d-md-block">
    <partner></partner>
  </section>
  <section class="statistics-holder bg-light py-5 d-none d-md-block border-t-r-white">
    <statistics></statistics>
  </section>

  <section class="subscribes-holder py-5 d-none d-md-block border-t-l-light">
    <Subscribes></Subscribes>
  </section>

  <section class="support-holder py-5 d-none d-md-block" id="supportSec">
    <Support></Support>
  </section>
</template>

<script>
import { mapGetters } from 'vuex'
import SwiperSlider from '../components/SwiperSlider'
import orderRecived from '../components/OrderRecived'
import statistics from '../components/Statistics.vue'
import Partner from '../components/Partners'
import Subscribes from '../components/Subscribes'
import Support from '../components/Support'

export default {
  name: 'Home',

  metaInfo: {
    titleTemplate: null
  },

  components: {
    SwiperSlider,
    orderRecived,
    Partner,
    statistics,
    Subscribes,
    Support
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
