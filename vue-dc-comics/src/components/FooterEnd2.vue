<template>
    <div>
        <div class="footerCard">
            <a class="bottom" href="#">SING-UP NOW!</a>
        </div>
        <div class="footerCard">
            <ul>
                <li class="bluSocial">FOLLOW US</li>
                <li v-for="social,index in socials" :key="index">
                    <a :href="social.link"><img :src="social.img" alt=""></a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name:'FooterEnd2',
    data(){
        return{
            socials:[
                {
                    img:require('../assets/img/footer-facebook.png'),
                    link:'#'
                },
                {
                    img:require('../assets/img/footer-twitter.png'),
                    link:'#'
                },
                {
                    img:require('../assets/img/footer-youtube.png'),
                    link:'#'
                },
                {
                    img:require('../assets/img/footer-pinterest.png'),
                    link:'#'
                },
                {
                    img:require('../assets/img/footer-periscope.png'),
                    link:'#'
                }
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
div{
    padding: 20px;
    position: relative;
    z-index: 14;
    display: flex;
    justify-content: space-between;
    background-color: hsl(0, 0%, 19%);
    .bluSocial{
        color: #0381e9;
    }
    .bottom{
        padding: 10px;
        text-decoration: none;
        color: white;
        border: 1px solid #0381e9;
    }
    ul{
        align-items: center;
        list-style: none;
        display: flex;
    }
    li{
        padding: 0 10px;
    }
}
</style>