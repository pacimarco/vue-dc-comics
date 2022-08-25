<template>
  <main>
      <section class="section-1">
          <h3>--> Content goes here --></h3>
          <div class="container comics-list">
              <div v-for="(card, index) in comicsList" :key="index"   class="comics-card">
                  <img :src="comicsList.thumb" alt="">
              <h3 class="title-comics">{{comicsList.series}}</h3>
              </div>
              
          </div>
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
                src: require('../assets/img/buy-comics-digital-comics.png'),
                text: 'DIGITAL COMICS',
            },
            {
                src: require('../assets/img/buy-comics-merchandise.png'),
                text: 'DC MERCHANDISE',
            },
            {
                src: require('../assets/img/buy-comics-subscriptions.png'),
                text: 'SUBSCRIPTION',
            },
            {
                src: require('../assets/img/buy-comics-shop-locator.png'),
                text: 'COMICS SHOP LOCATOR',
            },
            {
                src: require('../assets/img/buy-dc-power-visa.svg'),
                text: 'DC POWER VISA',
            }
        ],
        comicsList:[
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  }
]
    }
}
}
</script>

<style lang="scss">
.section-1{
    background-color: black;
    height: 630px;
    line-height: 130px;
    color: white;
    padding-left: 180px;

    .comics-list{
        display: flex;
        flex-wrap: wrap;
    }
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
        padding: 10px 20px;
        display: flex;
        align-items: center;
        
        
        
    }

    img{
        width: 35px;
        margin: 10px;
       
        
        
    }
}
.comics-card{
    flex-basis: 15%;

    img{
        max-width: 100%;
    }
}

</style>