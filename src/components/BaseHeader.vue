<template>
 <section class="nav-holder py-4">
    <div class="container">
    
        <nav class="navbar navbar-expand-md">
            
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarId"
                    aria-controls="navbarId" aria-expanded="false" aria-label="Toggle navigation">
                <span></span>
                <span></span>
                <span></span>
            </button>
    
            <div class="navbar-brand text-white d-md-none">الرئيسية</div>
            
            <a class="navbar-brand d-none d-md-inline-block" href="index.html" title="بلوبيز"><img src="https://via.placeholder.com/80x60" alt="Logo image"></a>
        
            <div class="collapse navbar-collapse" id="navbarId">
                <ul class="navbar-nav mr-auto">
                    <li class="nav-item active">
                        <a class="nav-link" title="الرئيسية" href="index.html">الرئيسية</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link smooth-a" title="طريقة الاستخدام" href="#aboutSec">طريقة الاستخدام</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" title="الطلبات" href="orders.html">الطلبات</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link smooth-a" title="الدعم والمساعده" href="#supportSec">الدعم والمساعده</a>
                    </li>
                </ul>
            </div>
    
            <ul class="navbar-nav mr-auto">
                <li class="nav-item px-md-2 d-none d-md-inline-block">
                    <a class="nav-link" title="بحث" href="openSearch">
                        <i class="icofont-search-1"></i>
                    </a>
                </li>
                <li class="nav-item d-none d-md-inline-block">
                    <a class="btn btn-primary btn-sm mt-1" title="الاشتراك" href="register.html">الاشتراك</a>
                </li>
                <!-- <li class="nav-item">
                    <a class="nav-link text-primary" title="الدخول" >
                        <span class="pl-2 d-md-none"><i class="icofont-user-alt-7"></i></span>الدخول
                    </a>
                    
                </li> -->
                <router-link :to="{ name: 'Login' }" class="nav-link text-primary" title="الدخول">
                  <span class="pl-2 d-md-none"><i class="icofont-user-alt-7"></i></span>الدخول
               </router-link>
               

            </ul>
    
            <div class="text-white d-md-none width-100 mt-5 mb-3">
                <p class="m-0">مرحبا</p>
            </div>
    
            <form method="post" action="search.html" class="search-form">
                <input type="search" placeholder="ابحث عما تريد">
                <button type="submit"><i class="icofont-search-1"></i></button>
            </form>
    
            <div class="mirror"></div>
            
        </nav>
        
    </div>
</section>
</template>

<script>
import { mapState, mapActions, mapGetters } from 'vuex'

export default {
//   data() {
//     return {
//       isLoginPage: false
//     };
//   },
//   created() {
//   // Simulate a delay using setTimeout
//   setTimeout(() => {
//     // Check if the current route is the login page
//     this.isLoginPage = this.$route.name === 'Login'; // Replace 'Login' with your actual login page route name
//   }, 2000); // This introduces a 3-second delay
// }

}
</script>

<style></style>
