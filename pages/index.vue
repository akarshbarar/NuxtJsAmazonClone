<template>
  <div class="container">
    <Header/>
    <HeaderTwo/>
    <div class="home">
        <img class="home__image" src="https://images-eu.ssl-images-amazon.com/images/G/02/digital/video/merch2016/Hero/Covid19/Generic/GWBleedingHero_ENG_COVIDUPDATE__XSite_1500x600_PV_en-GB._CB428684220_.jpg"/>
        <div class="home__row">
          <template v-for="block in content">
            <component :is="block.component" :block="block" :key="block.uid"></component>
          </template>
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
  },
  data(){
    return {
      content: []
    }
  },

  created(){
    this.content =[
      {
        uid:Math.random(),
        component: "Product",
        title: "Item 1",
        description: "Description 1",
        imageLink: "https://images-eu.ssl-images-amazon.com/images/G/02/digital/video/merch2016/Hero/Covid19/Generic/GWBleedingHero_ENG_COVIDUPDATE__XSite_1500x600_PV_en-GB._CB428684220_.jpg",
        rate:"5",
        price: "$100"
      },
       {
        uid:Math.random(),
        component: "Product",
        title: "Item 2",
        description: "Description 2",
        imageLink: "https://images-eu.ssl-images-amazon.com/images/G/02/digital/video/merch2016/Hero/Covid19/Generic/GWBleedingHero_ENG_COVIDUPDATE__XSite_1500x600_PV_en-GB._CB428684220_.jpg",
        rate:"5",
        price: "$200"
      },
        {
        uid:Math.random(),
        component: "Product",
        title: "Item 3",
        description: "Description 3",
        imageLink: "https://images-eu.ssl-images-amazon.com/images/G/02/digital/video/merch2016/Hero/Covid19/Generic/GWBleedingHero_ENG_COVIDUPDATE__XSite_1500x600_PV_en-GB._CB428684220_.jpg",
        rate:"5",
        price: "$300"
      },
{
        uid:Math.random(),
        component: "Product",
        title: "Item 1",
        description: "Description 1",
        imageLink: "https://images-eu.ssl-images-amazon.com/images/G/02/digital/video/merch2016/Hero/Covid19/Generic/GWBleedingHero_ENG_COVIDUPDATE__XSite_1500x600_PV_en-GB._CB428684220_.jpg",
        rate:"5",
        price: "$100"
      },
       {
        uid:Math.random(),
        component: "Product",
        title: "Item 2",
        description: "Description 2",
        imageLink: "https://images-eu.ssl-images-amazon.com/images/G/02/digital/video/merch2016/Hero/Covid19/Generic/GWBleedingHero_ENG_COVIDUPDATE__XSite_1500x600_PV_en-GB._CB428684220_.jpg",
        rate:"5",
        price: "$200"
      },
        {
        uid:Math.random(),
        component: "Product",
        title: "Item 3",
        description: "Description 3",
        imageLink: "https://images-eu.ssl-images-amazon.com/images/G/02/digital/video/merch2016/Hero/Covid19/Generic/GWBleedingHero_ENG_COVIDUPDATE__XSite_1500x600_PV_en-GB._CB428684220_.jpg",
        rate:"5",
        price: "$300"
      }, 
    ]
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

@media screen and (min-width: 1000px){
  .home__row{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(19rem,1fr));
  }
}
</style>
