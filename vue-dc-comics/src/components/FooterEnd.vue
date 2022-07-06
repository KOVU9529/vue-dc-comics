<template>
    <div class="container">
        <div class="listOne">
             <ul class="first">
            <li class="title">
                DC COMICS
            </li>
            <li v-for="first,index in firstLi" :key="index">
               <a :href="first.link"> {{first.text}}</a>
            </li>
        </ul>
        <ul class="second">

            <li class="title">
               SHOP
            </li>
            <li v-for="second,index in secondLi" :key="index">
                <a :href="second.link">{{second.text}}</a>
            </li>
        </ul>
       
        </div>
        <div class="listTwo">
             <ul class="first">
            <li class="title">
                DC 
            </li>
            <li v-for="third,index in thirdLi" :key="index">
               <a :href="third.link"> {{third.text}}</a>
            </li>
        </ul>
          <ul class="first">
            <li class="title">
                SITES
            </li>
            <li v-for="four,index in fourLi" :key="index">
               <a :href="four.link"> {{four.text}}</a>
            </li>
        </ul>
        </div>
        <div class="dc">
            
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            firstLi:[
                {
                    text:'Characters',
                    link:'#'
                },
                {
                    text:'Comics',
                    link:'#'
                },
                {
                    text:'Movies',
                    link:'#'
                },
                {
                    text:'TV',
                    link:'#'
                },
                {
                    text:'Games',
                    link:'#'
                },
                {
                    text:'Videos',
                    link:'#'
                },
                {
                    text:'News',
                    link:'#'
                },
            ],
            secondLi:[
                {
                    text:'Shop DC',
                    link:'#'
                },
                {
                    text:'Shop DC Collectibles',
                    link:'#'
                },
            ],
            thirdLi:[
                {
                    text:'Terms of use',
                    link:'#'
                },
                {
                    text:'Privacy Policy (New)',
                    link:'#'
                },
                {
                    text:'Ad choices',
                    link:'#'
                },
                {
                    text:'Advertising',
                    link:'#'
                },
                {
                    text:'Jobs',
                    link:'#'
                },
                {
                    text:'Subscriptions',
                    link:'#'
                },
                {
                    text:'Talent Workshops',
                    link:'#'
                },
                {
                    text:'CPSC Certificates',
                    link:'#'
                },
                {
                    text:'Ratings',
                    link:'#'
                },
                {
                    text:'Shop Help',
                    link:'#'
                },
                {
                    text:'Contact us',
                    link:'#'
                },
            ],
             fourLi:[
                {
                    text:'DC',
                    link:'#'
                },
                {
                    text:'MAD Magazine ',
                    link:'#'
                },
                {
                    text:'DC Kids',
                    link:'#'
                },
                {
                    text:'DC Universe',
                    link:'#'
                },
                {
                    text:'DC Power Visa',
                    link:'#'
                },
            ],
        }
        
    },
}
</script>
<style lang="scss" scoped>
.container{
    position: relative;
    background-image: url(../assets/img/footer-bg.jpg);
    height: 350px;
    display: flex;
    padding: 20px;
        .listTwo{
            padding: 0 20px;
            display: flex;
        }
        ul{
            padding: 0 20px;
            list-style-type: none;
             li{
                 margin-bottom: 5px;
               &.title{
                    color: white;
                    margin-top: 10px;
                    margin-bottom: 10px;
                }
                a{
                   text-decoration: none;
                   color: #737069;
                   font-size: 15px;
                }
            }
        }
    .dc{
        background-size: contain;
        background-image:url(../assets/img/dc-logo-bg.png);        
        position: absolute;
        z-index: 10;
        top: -25%;
        left: 60%;
        height: 500px;
        width: 500px;
    }
}
</style>