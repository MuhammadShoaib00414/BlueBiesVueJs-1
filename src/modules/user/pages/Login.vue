<template>
    <section class="win-height login-holder">
       <div class="form-holder bg-white px-lg-4 d-flex align-items-center">
           <div class="width-100 px-4 px-md-5">
       
               <!-- <img src="https://via.placeholder.com/80x60" alt="Logo image"> -->
               <h3 class="mt-3">تسجيل الدخول</h3>
               
               <form method="post" action="verification-code.html">
                   <label class="d-block">رقم الهاتف
                       <div class="input-group mb-2">
                           <div class="input-group-prepend">
                               <span class="input-group-text rounded-0 bg-white" id="basic-addon1">+966</span>
                           </div>
                           <input type="tel" class="form-control rounded-0" placeholder="اكتب رقم الهاتف" aria-describedby="basic-addon1">
                       </div>
                   </label>
                   
                   <label class="checkbox-holder d-block">
                       <input type="checkbox">
                       <span class="checkbox-icon"><i class="fa fa-check"></i></span>
                       <span>تذكرني</span>
                   </label>
                   
                   <router-link :to="{ name: 'Register' }" class="nav-link text-primary" title="الدخول">
                       <button type="submit" class="btn btn-primary">تسجيل الدخول</button>
                       <a  title="تسجيل حساب جديد" class="px-3">تسجيل حساب جديد</a>
                  </router-link>
                   <div class="my-3">
                      
                   </div>
               </form>
               
               <h5 class="mt-5">او تسجيل الدخول عن طريق</h5>
               <ul class="list-unstyled list-inline social">
                   <li class="list-inline-item m-0 ml-2"><a href="#" title="facebook"><i class="fab fa-facebook-f"></i></a></li>
                   <li class="list-inline-item m-0 ml-2"><a href="#" title="twitter"><i class="fab fa-twitter"></i></a></li>
                   <li class="list-inline-item m-0 ml-2"><a href="#" title="google+"><i class="fab fa-google-plus-g"></i></a></li>
               </ul>
               
           </div>
       </div>
   </section>
   </template>
   
   <script>
   export default {}
   </script>
   
   <style >
   section#base-header {
       display: none!important;;
   }
   footer#base-footer {
       display: none!important;;
   }
   .pre-load{
       display: block!important;
   }
   
   </style>
   
   