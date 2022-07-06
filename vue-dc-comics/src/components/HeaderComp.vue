<template>
    <header>
        <div>
            <img src="../assets/img/dc-logo.png" alt="DC logo">
        </div>
        <nav class="navHeader">
             <ul>
                <li v-for="link,index in links" :key="index"  >
                    <a :href="link.a" :class="{'active' : link.current}">{{link.text}}</a> 
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
            links:[
                {
                    text:'CARACTERS',
                    a:'#',
                    current:false
                },
                 {
                    text:'COMICS',
                    a:'#',
                    current:true
                },
                 {
                    text:'MOVIES',
                    a:'#',
                    current:false
                },
                {
                    text:'TV',
                    a:'#',
                    current:false
                },
                 {
                    text:'GAMES',
                    a:'#',
                    current:false
                },
                 {
                    text:'COLLECTIBLES',
                    a:'#',
                    current:false
                },
                 {
                    text:'VIDEOS',
                    a:'#',
                    current:false
                },
                 {
                    text:'FANS',
                    a:'#',
                    current:true
                },
                 {
                    text:'NEWS',
                    a:'#',
                    current:false
                },
                 {
                    text:'SHOP',
                    a:'#',
                    current:false
                }
            ],
        };
    }
}
</script>
<style lang="scss" scoped>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
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
    }
}
</style>
