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

    </div>
</footer>
</template>

<script>
export default {
name: 'MyFooter'
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
</style>