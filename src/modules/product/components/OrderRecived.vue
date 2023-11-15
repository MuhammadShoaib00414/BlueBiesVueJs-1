<template>

    <div class="container pt-md-4 pb-4 contain-filter">
        
        <div class="card text-white small-card bg-secondary d-md-none m-0 half-up">
            <div class="card-body">
                <i class="icofont-chart-line-alt"></i>
                <h5>ما الجديد</h5>
            </div>
        </div>
        
        <h2 class="mt-0 mb-4 d-none d-md-block">جديد الطلبات الواردة</h2>
        
        <div class="row d-none d-md-flex mb-3">
            <div class="col-md-6 filter-btns">
                <button type="button" class="btn btn-sm" data-filter="all"><i class="icofont-ghost ml-1"></i>الكل</button>
                <button type="button" class="btn btn-sm" data-filter=".food"><i class="icofont-food-basket ml-1"></i>الاطعمة</button>
                <button type="button" class="btn btn-sm" data-filter=".car"><i class="icofont-car ml-1"></i>السيارات</button>
            </div>
            <div class="col-md-6 text-left">
                <div class="select-with-icon">
                    <select>
                        <option>تصفية الطلبات</option>
                        <option value="1">1</option>
                        <option value="2">2</option>
                        <option value="3">3</option>
                    </select>
                    <i class="icofont-filter"></i>
                </div>
                <div class="select-with-icon">
                    <select>
                        <option>ترتيب حسب</option>
                        <option value="1">1</option>
                        <option value="2">2</option>
                        <option value="3">3</option>
                    </select>
                    <i class="fa fa-sort-amount-down"></i>
                </div>
            </div>
        </div>
        
        <div class="row">
            
            <div class="col-md-6 col-lg-4 mix food">
                <div class="animate-box">
                    <div class="card bg-primary text-white">
                        <div class="card-body py-4 countdown" data-expire="2020/6/5">
                            <div class="row m-0">
                                <div class="col-9 p-0"><h3 class="">تأمين صحي</h3></div>
                                <div class="col-3 p-0">
                                    <span class="font-2x d-block">350</span> زيارة
                                </div>
                            </div>
                            
                            <p class="mt-4 mb-0">متبقي على العرض</p>
                            <div class="details counter-holder row m-0 mb-4">
                                <div class="col p-0">
                                    <span class="day font-2x d-block"></span>
                                    <small>يوم</small>
                                </div>
                                <div class="col p-0">
                                    <span class="hours font-2x d-block"></span>
                                    <small>ساعه</small>
                                </div>
                                <div class="col p-0">
                                    <span class="minutes font-2x d-block"></span>
                                    <small>دقيقة</small>
                                </div>
                                <div class="col p-0">
                                    <span class="seconds font-2x d-block"></span>
                                    <small>ثانية</small>
                                </div>
                            </div>
                            
                            <a href="add-offer.html" title="تقدم بعرض الان" class="btn btn-sm btn-outline-white">تقدم بعرض الان</a>
                            
                            <a href="order-single.html" title="التفاصيل" class="order-btn"><i class="fa fa-chevron-left"></i> التفاصيل</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="col-md-6 col-lg-4 mix food">
                <div class="animate-box">
                    <div class="card">
                        <div class="card-body py-4">
                            <div class="row">
                                <div class="col"><span class="round-icon"><i class="fa fa-city"></i></span></div>
                                <div class="col text-left">
                                    <a href="#" title="طلب عرض اسعار" class="btn btn-sm btn-outline-light mt-1">طلب عرض اسعار</a>
                                </div>
                            </div>
                            
                            <h3 class="mt-4 mb-5">تأمين صحي</h3>
                            
                            <ul class="list-unstyled list-inline text-muted">
                                <li class="list-inline-item m-0"><i class="icofont-google-map ml-1"></i> الرياض</li>
                                <li class="list-inline-item mr-2"><i class="icofont-clock-time ml-1"></i> <span class="d-inline-block"> 14 اغسطس, 2019</span></li>
                            </ul>
                            
                            <img src="images/order-logo-1.png" alt="logo" class="order-logo">
                            
                            <a href="order-single.html" title="التفاصيل" class="order-btn"><i class="fa fa-chevron-left"></i> التفاصيل</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="col-md-6 col-lg-4 mix car">
                <div class="animate-box">
                    <div class="card">
                        <div class="card-body py-4">
                            <div class="row">
                                <div class="col"><span class="round-icon"><i class="fa fa-city"></i></span></div>
                                <div class="col text-left">
                                    <a href="#" title="طلب عرض اسعار" class="btn btn-sm btn-outline-light mt-1">طلب عرض اسعار</a>
                                </div>
                            </div>
                            
                            <h3 class="mt-4 mb-5">تأمين صحي</h3>
                            
                            <ul class="list-unstyled list-inline text-muted">
                                <li class="list-inline-item m-0"><i class="icofont-google-map ml-1"></i> الرياض</li>
                                <li class="list-inline-item mr-2"><i class="icofont-clock-time ml-1"></i> <span class="d-inline-block"> 14 اغسطس, 2019</span></li>
                            </ul>
                            
                            <img src="images/order-logo-1.png" alt="logo" class="order-logo">
                            
                            <a href="order-single.html" title="التفاصيل" class="order-btn"><i class="fa fa-chevron-left"></i> التفاصيل</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="col-md-6 col-lg-4 mix food">
                <div class="animate-box">
                    <div class="card">
                        <div class="card-body py-4">
                            <div class="row">
                                <div class="col"><span class="round-icon"><i class="fa fa-city"></i></span></div>
                                <div class="col text-left">
                                    <a href="#" title="طلب عرض اسعار" class="btn btn-sm btn-outline-light mt-1">طلب عرض اسعار</a>
                                </div>
                            </div>
                            
                            <h3 class="mt-4 mb-5">تأمين صحي</h3>
                            
                            <ul class="list-unstyled list-inline text-muted">
                                <li class="list-inline-item m-0"><i class="icofont-google-map ml-1"></i> الرياض</li>
                                <li class="list-inline-item mr-2"><i class="icofont-clock-time ml-1"></i> <span class="d-inline-block"> 14 اغسطس, 2019</span></li>
                            </ul>
                            
                            <img src="images/order-logo-1.png" alt="logo" class="order-logo">
                            
                            <a href="order-single.html" title="التفاصيل" class="order-btn"><i class="fa fa-chevron-left"></i> التفاصيل</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="col-md-6 col-lg-4 mix food">
                <div class="animate-box">
                    <div class="card">
                        <div class="card-body py-4">
                            <div class="row">
                                <div class="col"><span class="round-icon"><i class="fa fa-city"></i></span></div>
                                <div class="col text-left">
                                    <a href="#" title="طلب عرض اسعار" class="btn btn-sm btn-outline-light mt-1">طلب عرض اسعار</a>
                                </div>
                            </div>
                            
                            <h3 class="mt-4 mb-5">تأمين صحي</h3>
                            
                            <ul class="list-unstyled list-inline text-muted">
                                <li class="list-inline-item m-0"><i class="icofont-google-map ml-1"></i> الرياض</li>
                                <li class="list-inline-item mr-2"><i class="icofont-clock-time ml-1"></i> <span class="d-inline-block"> 14 اغسطس, 2019</span></li>
                            </ul>
                            
                            <img src="images/order-logo-1.png" alt="logo" class="order-logo">
                            
                            <a href="order-single.html" title="التفاصيل" class="order-btn"><i class="fa fa-chevron-left"></i> التفاصيل</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="col-md-6 col-lg-4 mix car">
                <div class="animate-box">
                    <div class="card">
                        <div class="card-body py-4">
                            <div class="row">
                                <div class="col"><span class="round-icon"><i class="fa fa-city"></i></span></div>
                                <div class="col text-left">
                                    <a href="#" title="طلب عرض اسعار" class="btn btn-sm btn-outline-light mt-1">طلب عرض اسعار</a>
                                </div>
                            </div>
                            
                            <h3 class="mt-4 mb-5">تأمين صحي</h3>
                            
                            <ul class="list-unstyled list-inline text-muted">
                                <li class="list-inline-item m-0"><i class="icofont-google-map ml-1"></i> الرياض</li>
                                <li class="list-inline-item mr-2"><i class="icofont-clock-time ml-1"></i> <span class="d-inline-block"> 14 اغسطس, 2019</span></li>
                            </ul>
                            
                            <img src="images/order-logo-1.png" alt="logo" class="order-logo">
                            
                            <a href="order-single.html" title="التفاصيل" class="order-btn"><i class="fa fa-chevron-left"></i> التفاصيل</a>
                        </div>
                    </div>
                </div>
            </div>
            
        </div>
        
        <div class="text-md-left animate-box right-in mt-3">
            <span class="d-none d-md-inline-block">يوجد أكثر من 40 طلب</span>
            <a href="orders.html" class="btn btn-primary mr-2" title="عرض كافة الطلبات">عرض كافة الطلبات <i class="icofont-arrow-left mr-1"></i></a>
        </div>
        
    </div>
 
</template>

<script>
export default {
  data() {
    return {
      partnerCompanies: [
        {
          name: "اسم الشركة 1",
          image: "images/company-1.png",
          link: "#"
        },
        {
          name: "اسم الشركة 2",
          image: "images/company-2.png",
          link: "#"
        },
        {
          name: "اسم الشركة 3",
          image: "images/company-3.png",
          link: "#"
        },
        {
          name: "اسم الشركة 4",
          image: "images/company-4.png",
          link: "#"
        },
        // Add more partner companies as needed
      ]
    };
  }
};
</script>

<style></style>
