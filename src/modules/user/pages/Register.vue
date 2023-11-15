<template>
  <section class="win-height login-holder">
    <div class="form-holder bg-white px-lg-4 d-flex align-items-center">
      <div class="width-100 px-4 px-md-5">

        <img src="https://via.placeholder.com/80x60" alt="Logo image">
        <h3 class="mt-3">تسجيل عضوية جديدة</h3>

        <form method="post" @submit.prevent="registerUser">
          <label class="d-block">اسم المستخدم
            <input type="text" placeholder="اسم المستخدم" class="border rounded-0">
          </label>

          <label class="d-block">رقم الهاتف
            <div class="input-group mb-2">
              <div class="input-group-prepend">
                <span class="input-group-text rounded-0 bg-white" id="basic-addon1">+966</span>
              </div>
              <input type="tel" class="form-control rounded-0" placeholder="اكتب رقم الهاتف"
                aria-describedby="basic-addon1">
            </div>
          </label>

          <label class="d-block">البريد الالكتروني
            <input type="email" placeholder="البريد الالكتروني" class="border rounded-0">
          </label>

          <label class="d-block">كلمة المرور
            <input type="password" placeholder="كلمة المرور" class="border rounded-0">
          </label>

          <label class="d-block">تأكيد كلمة المرور
            <input type="password" placeholder="تأكيد كلمة المرور" class="border rounded-0">
          </label>

          <div>
            <label class="radio-holder">
              <input type="radio" checked>
              <span class="radio-icon"><i class="fa fa-check"></i></span>
              <span>مقدم الخدمة</span>
            </label>
            <label class="radio-holder mr-2">
              <input type="radio">
              <span class="radio-icon"><i class="fa fa-check"></i></span>
              <span>طالب الخدمة</span>
            </label>
          </div>

          <div class="my-3">
            <button type="submit" class="btn btn-primary">تسجيل حساب جديد</button>
            <a href="login.html" title="تسجيل حساب جديد" class="px-3">تسجيل الدخول</a>
          </div>
        </form>

        <!-- <h5 class="mt-5">او تسجيل عن طريق</h5>
            <ul class="list-unstyled list-inline social">
                <li class="list-inline-item m-0 ml-2"><a href="#" title="facebook"><i class="fab fa-facebook-f"></i></a></li>
                <li class="list-inline-item m-0 ml-2"><a href="#" title="twitter"><i class="fab fa-twitter"></i></a></li>
                <li class="list-inline-item m-0 ml-2"><a href="#" title="google+"><i class="fab fa-google-plus-g"></i></a></li>
            </ul> -->

      </div>
    </div>
  </section>
</template>

<script>
import axios from 'axios';

export default {
  data() {
    return {
      username: '',
      phoneNumber: '',
      email: '',
      password: '',
      confirmPassword: '',
      userType: 'provider', // Default to 'provider', you can change this based on your requirements
    };
  },
  methods: {
  async registerUser() {
    alert('test')
    try {
      // Use proxy in development
      const baseUrl = process.env.NODE_ENV === 'development' ? 'http://localhost:8000' : '';

      // Add the withCredentials option
      const response = await axios.post(`${baseUrl}/api/v1/auth/register`, {
        username: this.username,
        phoneNumber: `+966${this.phoneNumber}`, // Assuming you want to include the country code
        email: this.email,
        password: this.password,
        confirmPassword: this.confirmPassword,
        userType: this.userType,
      }, {
        withCredentials: true, // Include credentials (cookies, authentication)
        headers: {
          'Access-Control-Allow-Origin': '*', // Replace * with your actual origin in production
          // ... other headers
        },
      });

      // Handle the response as needed, for example, you can redirect the user to a verification page
      console.log(response.data);
    } catch (error) {
      console.error('Error during registration:', error);
      // Handle the error (e.g., show an error message to the user)
    }
  },
},

};
</script>


<style >
section#base-header {
  display: none !important;
  ;
}

footer#base-footer {
  display: none !important;
  ;
}

.pre-load {
  display: block !important;
}</style>
