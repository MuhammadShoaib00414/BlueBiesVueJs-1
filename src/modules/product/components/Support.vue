<template>
  <div class="container pb-5 pt-4">
    <div class="row">

      <div class="col-md-6">
        <h3 class="mt-0 mb-4">الدعم والمساعدة</h3>

        <div class="supportAccordion">

          <div class="card animate-box active" v-for="(data, index) in faqs" :key="index">

            <div v-if="data.status == 1" class="card-header" @click="toggleAccordion(index)">
              {{ data.question }}
              <i class="fa fa-chevron-down" :class="{ 'fa-chevron-up': activeIndex === index }"></i>
            </div>
            <div class="card-body" v-show="activeIndex === index">{{ data.answer }}</div>
          </div>

          <!-- <div class="card animate-box">
            <div class="card-header">هل انتم تبيعون منتج؟
              <i class="fa fa-chevron-down"></i>
            </div>
            <div class="card-body">بلوبيز تخدم جميع قطاعات الاعمال التجارية وتخلق سوق موازي وتستهدف خدمات منشأتك عن طريق
              المنشآت التي تتعامل داخل منصه بلوبيز</div>
          </div>
          <div class="card animate-box">
            <div class="card-header">كيف اتأكد من مصداقية منصتكم؟
              <i class="fa fa-chevron-down"></i>
            </div>
            <div class="card-body">بلوبيز تخدم جميع قطاعات الاعمال التجارية وتخلق سوق موازي وتستهدف خدمات منشأتك عن طريق
              المنشآت التي تتعامل داخل منصه بلوبيز</div>
          </div> -->
        </div>
      </div>
      
      <div class="col-md-1"></div>

      <div class="col-md-5">
        <h3 class="mt-0 mb-4">التواصل مع بلوبيز</h3> 

        <ul class="list-unstyled">
          <li class="animate-box"><i class="icofont-phone font-2x"></i></li>
          <li class="animate-box">عن طريق الاتصال بنا</li>
          <li class="animate-box"><a href="tel:+9660513123124" class="font-1x ltr d-inline-block">{{ contacts.phoneNumber }}</a>
          </li>
          <li class="animate-box mt-1"><i class="icofont-mail font-2x"></i></li>
          <li class="animate-box">عن طريق إرسال بريد الكتروني</li>
          <li class="animate-box"><a href="mailto:hello@blue-bees.com" class="font-1x">{{ contacts.email }}</a></li>
        </ul>

        <div class="animate-box"><a href="dashboard-support-add.html" class="btn btn-primary" title="فتح تذكرة دعم فني"><i
              class="fa fa-plus ml-1"></i> فتح تذكرة دعم فني</a></div>
      </div>

    </div>
  </div>
</template>

<script>
import axios from 'axios';
export default {
  data() {
    return {
      contacts: '',
      faqs: [],
      activeIndex: 0, // Initially, the first card is active
    };
  },
  created() {
    // Fetch data from the API when the component is created
    axios
      .get('http://127.0.0.1:8000/api/v1/faqs-data')
      .then((response) => {
        // Update the partnerCompanies array with the data from the API
        this.faqs = response.data.faqs;
        this.contacts = response.data.contacts;
        console.log('contacts', this.contacts);
      })
      .catch((error) => {
        console.er
        ror('Error fetching data from the API', error);
      });
  },
  methods: {
    toggleAccordion(index) {
      if (this.activeIndex === index) {
        this.activeIndex = -1; // Close the active card if clicked again
      } else {
        this.activeIndex = index; // Open the clicked card
      }
    }
  },
};
</script>

<style></style>
 