<template>
<footer>
    <div class="top-footer">
        <div class="left-ftr">
            <h4>DC COMICS</h4>
            <ul>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">Tv</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Video</a></li>
                <li><a href="#">News</a></li>
            </ul>
            <h4>SHOP</h4>
            <ul>
                <li><a href="">SHOP DC</a></li>
                <li><a href="#">Shop Dc Coleectibles</a></li>
            </ul>
        </div>
        <div class="center-ftr">
            <h4>DC</h4>
            <ul>
                <li> <a href="#">Terms of use</a></li>
                <li><a href="#">Privacy pollicy (New)</a></li>
                <li><a href="#">Ad Choices</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">Subscriptions</a></li>
                <li><a href="#">Subscriptions</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Ratings</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact US</a></li>
            </ul>
        </div>
        <div class="right-ftr">
            <h4>SITIES</h4>
            <ul>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">Dc Power visa</a></li>
            </ul>
        </div>
        <img class="logo-footer" src="../assets/img/dc-logo-bg.png" alt="">
    </div>
    
    <div class="bottom-footer">
        <div class="sign-up">
            <button>SIGN-UP NOW</button>
        </div>
        <div class="app">
            <h4>FOLLOW US</h4>
            <ul>
                <li v-for="(app, index) in app" :key="index">
                    <a :href="app.at">
                    <img :src="app.src" alt="">
                    </a>
                </li>
            </ul>
        </div>
    </div>
</footer>
</template>

<script>
export default {
name: 'MyFooter',
data(){
    return{
        app:[
            {
                src: require('../assets/img/footer-facebook.png'),
                at: '#',
            },
            {
                src: require('../assets/img/footer-twitter.png'),
                at: '#',
            },
            {
                src: require('../assets/img/footer-youtube.png'),
                at: '#',
            },
            {
                src: require('../assets/img/footer-pinterest.png'),
                at: '#',
            },
            {
                src: require('../assets/img/footer-periscope.png'),
                at: '#',
            }
        ]
    }
}
}
</script>

<style lang="scss">
.top-footer{
    background-image: url('../assets/img/footer-bg.jpg');
    height: 350px;
    display: flex;
    padding-top: 20px;
    justify-content: flex-start;
    padding-left: 50px;

    h4{
        color: white;
        margin: 5px 25px;
        
    }
    li{
        
        font-size: 9px;
        list-style: none;
        margin:5px 20px;
        padding: 5px 5px;

        a{
            text-decoration: none;
            color: gray;
        }
    }
    .logo-footer{
        margin-left: 150px;
    }
}
.bottom-footer{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 110px;
    background-color: rgb(42, 42, 48);

    button{
    color:white;
     background-color: rgb(42, 42, 48);
     padding: 10px;
     border: 2px solid rgb(12,105,247);
     margin-left: 150px;
    }

    .app{
        display: flex;
        justify-content: center;
        align-items: center;
        width: 50%;

        h4{
            color: rgb(12,105,247);
        }


        ul{
            list-style: none;

            li{
                
                display: inline-block;
                

                a{
                    text-decoration: none;
                    padding:10px;

                    img{
                        width: 25px;
                    }
                }
            }
        }
    }
}
</style>