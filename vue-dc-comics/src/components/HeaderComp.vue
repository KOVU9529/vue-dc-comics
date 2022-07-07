<template>
    <header>
        <div>
            <img src="../assets/img/dc-logo.png" alt="DC logo">
        </div>
        <nav class="navHeader">
             <ul>
                <li   v-for="link,index in links" :key="index"  >
                    <a  @click="active(index)" :href="link.a" :class="{'active' : index === currentActiveElement}">{{link.text}}</a> 
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name:"HeaderComp",
    data(){
        
        return {
            currentActiveElement:0,
            links:[
                {
                    text:'CARACTERS',
                    a:'#',
                },
                 {
                    text:'COMICS',
                    a:'#',   
                },
                 {
                    text:'MOVIES',
                    a:'#',
                },
                {
                    text:'TV',
                    a:'#',
                },
                 {
                    text:'GAMES',
                    a:'#',
                },
                 {
                    text:'COLLECTIBLES',
                    a:'#',
                },
                 {
                    text:'VIDEOS',
                    a:'#',
                },
                 {
                    text:'FANS',
                    a:'#',
                },
                 {
                    text:'NEWS',
                    a:'#',
                },
                 {
                    text:'SHOP',
                    a:'#',
                }
            ],
        };
    },
    methods:{
        active (index){
          this.currentActiveElement=index;
        }
    }
}
</script>
<style lang="scss" scoped>

header{
    height: 150px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .navHeader{
         height: 100%;
        ul{
         height: 100%;
         list-style-type: none;
         display: flex;
            li{
                height: 100%;
                display: flex;
                align-items: center;
                padding: 0 20px;
             a{
                height: 100%;
                display: flex;
                align-items: center;
                text-decoration: none;
                color: inherit;
                &.active{
                color: #4f93fa;
                border-bottom:3px solid  #4f93fa;
             }
            }
        }
    }
    img{
        padding: 30px
    };
}
}
</style>
