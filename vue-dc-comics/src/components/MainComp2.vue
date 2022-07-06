<template>
    <div>
        <ul>
            <li v-for="icon,index in icons" :key="index"  >
                <img :src="icon.img" alt="">
                <a :href="icon.a" >{{icon.text}}</a> 
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name:"MainComp2",
    data() {
        return {
            icons:[
                {
                    img:require('../assets/img/buy-comics-digital-comics.png'),
                    text:'DIGITAL COMICS',
                    a:'#'
                },
                {
                    img:require('../assets/img/buy-comics-merchandise.png'),
                    text:'DC MERCHANDISE',
                    a:'#'
                },
                {
                    img:require('../assets/img/buy-comics-subscriptions.png'),
                    text:'SUBSCRIPTION',
                    a:'#'
                },
                {
                    img:require('../assets/img/buy-comics-shop-locator.png'),
                    text:'COMIC SHOP LOCATOR',
                    a:'#'
                },
                {
                    img:require('../assets/img/buy-dc-power-visa.svg'),
                    text:'DC POWER VISA',
                    a:'#'
                }
            ],
        }; 
    }
}
</script>
<style lang="scss" scoped>
div{
    position: relative;
    z-index: 12;
    height: 130px;
    background-color: #0182fa;
    ul{
        height: 100%;
        list-style-type: none;
        display: flex;
        justify-content: center;
        li{
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
          a{
            text-decoration: none;
            color: white;
           }
        }
    }
    img{
        width: 60px;
        padding: 0 10px;
    }
}
</style>