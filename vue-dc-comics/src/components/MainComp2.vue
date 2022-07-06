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
                    img:'../assets/img/buy-comics-digital-comics.png',
                    text:'DIGITAL COMICS',
                    a:'#'
                },
                {
                    img:'../assets/img/buy-merchandise.png',
                    text:'DC MERCHANDISE',
                    a:'#'
                },
                {
                    img:'../assets/img/buy-subscriptions.png',
                    text:'SUBSCRIPTION',
                    a:'#'
                },
                {
                    img:'../assets/img/buy-comics-shop-locator.png',
                    text:'COMIC SHOP LOCATOR',
                    a:'#'
                },
                {
                    img:'../assets/img/buy-dc-power-visa.svg',
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
    height: 300px;
    background-color: #0182fa;
    ul{
        list-style-type: none;
        display: flex;
        li{
            padding: 20px;

          a{
            text-decoration: none;
            color: white;
           }
        }
    }
}
</style>