<template>
  <footer class="py-4 d-none d-md-block">
    <div class="container pt-3 ">
      <div class="row">
        <div class="col-8">
          <div class="media">
            <img src="https://via.placeholder.com/80x60" class="align-self-center ml-3" alt="...">
            <div class="media-body">
              <h5 class="m-0">بلوبيز</h5>
              <small>جميع الحقوق محفوظة 2019</small>
            </div>
          </div>
        </div>

        <div class="col-4 text-left">
          <ul class="list-unstyled list-inline social m-0">
            <li class="list-inline-item">
              <a href="#" title="facebook"><i class="icofont-facebook"></i></a>
            </li>
            <li class="list-inline-item">
              <a href="#" title="twitter"><i class="icofont-twitter"></i></a>
            </li>
            <li class="list-inline-item">
              <a href="#" title="linkedin"><i class="fab fa-linkedin-in"></i></a>
            </li>
          </ul>
        </div>
      </div>

      <ul class="list-unstyled list-inline mb-0 mt-4">
        <li class="list-inline-item m-0 pl-4"><a href="index.html" title="الرئيسية">الرئيسية</a></li>
        <li class="list-inline-item m-0 pl-4"><a href="blog.html" title="المدونة">المدونة</a></li>
        <li class="list-inline-item m-0 pl-4"><a href="orders.html" title="الطلبات">الطلبات</a></li>
        <li class="list-inline-item m-0 pl-4"><a href="faq.html" title="الاسئلة الشائعة">الاسئلة الشائعة</a></li>
        <li class="list-inline-item m-0 pl-4"><a href="contact.html" title="اتصل بنا">اتصل بنا</a></li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'BaseFooter',

  props: {
    showSideBar: {
      type: Boolean,
      required: true
    }
  },

  // data() {
  //   return {
  //     isLoginPage: false
  //   };
  // },
  // created() {
  //   // Check if the current route is the login page
  //   this.isLoginPage = this.$route.name === 'Login'; // Replace 'Login' with your actual login page route name
  //   alert(this.isLoginPage);
  // }

}
</script>

<style></style>
