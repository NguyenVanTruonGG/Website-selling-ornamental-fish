<template>
    <div class="wrapper">
       <div class="header">
          <div class="nav-menu">
             <NavMenu />
          </div>
       </div>
       <div class="container">
          <p>
             <i class="fa-solid fa-location-dot"></i>
             <a href="https://ctu.edu.vn">
                Trường Đại Học Cần Thơ Khu II, Đường 3/2, Xuân Khánh, Ninh Kiều, Cần
                Thơ
             </a>
          </p>
          <p>
             <i class="fa-solid fa-school"></i>
             Trường Công Nghệ Thông Tin Và Truyền Thông
          </p>
          <p>
             <i class="fa-solid fa-envelope icon-email"></i>
             Subin@gmail.com
          </p>
          <p>
             <i class="fa-solid fa-phone icon-phone"></i>
             0794388536
          </p>
         
          <div class="form-group row">
             <label class="col-sm-2 col-form-label">Đóng góp ý kiến</label>
             <div class="col-sm-8">
                <textarea class="form-control" row="7"> </textarea>
                <button
                   type="submit"
                   class="btn btn-primary mt-2 float-left"
                   @click="feedback"
                >
                   Gửi
                </button>
                <button type="reset" class="btn btn-danger mt-2 ml-2 float-left">
                   Xóa
                </button>
             </div>
          </div>
       </div>
    </div>
 </template>
 
 <script>
 import NavMenu from "../components/NavMenu.vue";
 
 export default {
    components: {
       NavMenu,
    },
    methods: {
       feedback() {
          alert("Cảm ơn bạn đã đóng góp ý kiến!!");
       },
    },
 };
 </script>
 
 <style scoped>
 .wrapper {
    max-width: 100%;
    background-color: #fff;
    font-family: "Open Sans", sans-serif;
    padding-bottom: 50px;
 }
 .header {
    width: 100%;
    height: auto;
 }
 .container {
    text-align: center;
    margin-top: 10px;
    color: #333;
 }
 </style>
 