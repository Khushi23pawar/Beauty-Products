<template>
  <!-- start navbar coading -->
  <nav class="navbar navbar-expand-lg   navbar-light top-menu fixed-top ">
         <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#nav-slider">
         <span class="navbar-toggler-icon"></span>
         </button>
         <!-- bar and close icon -->
         <div class="logo-container">
            <a href="#" class="navbar-brand logo-desktop d-none d-md-none d-lg-block">
            <img src="https://meowmeowtweet.com/cdn/shop/files/MMT_Logos_Primary_Logo_e0d772f6-be9c-4238-ae00-ed2bf1a2f03e_110x.png?v=1655960410"
               alt="logo" class="img-fluid logo-img"></a>
         </div>
         <div class="collapse navbar-collapse" id="nav-slider">
            <ul class="navbar-nav">
               <li class="nav-item dropdown mega-menu">
                  <a href="#" class="nav-link dropdown-toggle"  id="navbarDropdown"  role="button" data-toggle="dropdown"
                     aria-haspopup="true" aria-expanded="false">Shop</a>
                  <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                     <div class="row" style="flex-direction:column">
                        <div class="col-md-3">
                           <h5>Pits</h5>
                           <a class="dropdown-item" href="#">Deodornant Creams</a>
                           <a class="dropdown-item" href="#">Deodornant Sticks </a>
                           <a class="dropdown-item" href="#">Sensitive Skin</a>
                        </div>

                     </div>
                  </div>
               </li>
               <li class="nav-item"><a href="#" class="nav-link">Who We Are</a></li>
               <li class="nav-item"><a href="#" class="nav-link">Blog</a></li>
               <li class="nav-item"><a href="#" class="nav-link">FAQ</a></li>
               <li class="nav-item"><a href="#" class="nav-link">Refill Program</a></li>
               <li class="nav-item"><a href="#" class="nav-link">Reward Program</a></li>
            </ul>
         </div>
         <div class="fafa-icon">
            <i class="fa fa-user-circle"></i>
            <i class="fa fa-search px-3"></i>
            <i class="fa fa-shopping-bag"></i>
         </div>
         <!-- <button type="button" class="btn sec-font sec-color nav-font d-none d-lg-block sign_up_button">Sign Up</button> -->
      </nav>
</template>

<script>
export default{
  name: 'HeaderCom',
  
}
</script>

<style scoped>


 
</style>