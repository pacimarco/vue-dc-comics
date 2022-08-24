<template>
  <main>
      <section class="section-1">
          <h3>--> Content goes here --></h3>
      </section>

      <section class="section-2">
          <div class="main-menu" v-for="(menu, index) in menu" :key="index">
              <img :src="menu.src" alt="menu">
              {{menu.text}}

          </div>

      </section>
  </main>
</template>

<script>


export default {
name: 'MyMain',
data(){
    return{
        menu:[
            {
                src: '../assets/img/buy-comics-digital-comics.png',
                text: 'DIGITAL COMICS',
            },
            {
                src: '../assets/img/buy-comics-merchandise.png',
                text: 'DC MERCHANDISE',
            },
            {
                src: '../assets/img/buy-comics-subscription.png',
                text: 'SUBSCRIPTION',
            },
            {
                src: '../assets/img/buy-comics-shop-locator.png',
                text: 'COMICS SHOP LOCATOR',
            },
            {
                src: '../assets/img/buy-dc-power-visa.svg',
                text: 'DC POWER VISA',
            }
        ]
    }
}
}
</script>

<style lang="scss">
.section-1{
    background-color: black;
    height: 130px;
    line-height: 130px;
    color: white;
    padding-left: 180px;
}
.section-2{
    background-color: rgb(12,105,247);
    display: flex;
    font-size: 11px;
    justify-content: center;
    height: 150px;
    align-items: center;
    line-height: 150px;
    color: white;
    
    .main-menu{
        padding: 0 20px;
    }
}

</style>