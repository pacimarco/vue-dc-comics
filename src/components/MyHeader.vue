<template>
  
      <header>
          <img src="../assets/img/dc-logo.png" alt="logo">
          <ul>
              <li v-for="(link, index) in links" :key="index">
                  <a :href="link.url" :class="link.active?'active': ''">{{link.text}}</a>
              </li>
              
          </ul>
      </header>
  
</template>

<script>
export default {
name: 'MyHeader',
data(){
    return{
        links:[
            {
                text: 'CHARACTERS',
                url: '#',
                active: false
            },
            {
                text: 'COMICS',
                url: '#',
                active: true
            },
            {
                text: 'MOVIES',
                url: '#',
                active: false
            },
            {
                text: 'TV',
                url: '#',
                active: false
            },
            {
                text: 'GAMES',
                url: '#',
                active: false
            },
            {
                text: 'COLLECTIBLES',
                url: '#',
                active: false
            },
            {
                text: 'VIDEOS',
                url: '#',
                active: false
            },
            {
                text: 'FANS',
                url: '#',
                active: false
            },
            {
                text: 'NEWS',
                url: '#',
                active: false
            },
            {
                text: 'SHOP',
                url: '#',
                active: false
            },
        ]
    }
}
}
</script>

<style lang="scss">
header{
    text-align: center;
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 20px;

    img{
        width: 60px;
    }

    ul{
        list-style: none;
        margin: 20px;

        li{
            display: inline-block;
            margin: 0 10px;

            a{
                text-decoration: none;
                font-size: 10px;
                color: black;
                padding: 10px;

                &.active, &:hover{
                    border-bottom: 2px solid blue;
                }
            }
        }
        
    }
}
</style>