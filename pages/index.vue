<template>
  <div class="container">
    <Header/>
    <HeaderTwo/>
    <div class="home">
        <img class="home__image" src="https://images-eu.ssl-images-amazon.com/images/G/02/digital/video/merch2016/Hero/Covid19/Generic/GWBleedingHero_ENG_COVIDUPDATE__XSite_1500x600_PV_en-GB._CB428684220_.jpg"/>
        <div class="home__row">
          <Product/>
        </div>
    </div>

  </div>
</template>

<script>
import Header from '../layouts/partials/Navbar.vue';
import HeaderTwo from '../layouts/partials/NavbarTwo.vue';
import Product  from '../components/Product.vue';
export default {
  components:{
    Header,
    HeaderTwo,
    Product
  }
}
</script>

<style>
.home{
  max-width:1500px ;
  margin-left: auto;
  margin-right: auto;
  color: white;
}
.home__image{
  mask-image: linear-gradient(to bottom,rgba(0,0,0,1),rgba(0,0,0,0));
  width:100%;
  margin-bottom: -150px;
  z-index: -1;
}

.home__row{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  z-index: 1;
  max-width: 1500px;
  margin: 0 5px;
}
</style>
