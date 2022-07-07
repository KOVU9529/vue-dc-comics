<template>
    <section>
        <div class="container-dc">
            <div class="dc-list">
                <DcCard v-for="element,index in listDc" :key="index" :dcDetails="element"/>
            </div>
            <a class="button" href="#">LOAD MORE</a>
            <a class="button translate" href="#">CURRENT SERIES</a>
        </div>
    </section>
</template>

<script>
import  DcComic  from '../assets/Filejason/dc-comics.json';
import  DcCard  from './DcCard.vue';

export default ({
    name:'DcList',
    components:{
        DcCard
    },
    data(){
        return{
            listDc:DcComic
        }
    }
    });
</script>

<style lang="scss" scoped>
      section{
          .container-dc{
              position: relative;
              margin: 0 auto;
              width: 100%;
              padding: 0 15%;
              padding-top: 3% ;
              padding-bottom: 2%;
              background-color:#1c1c1c ;
              text-align: center;
              
          .dc-list{
              padding:0 10%;    
              display: flex;
              flex-wrap: wrap;
              text-align: left;
            }
            .button{
                background-color: #0182fa;
                text-decoration: none;
                color: white;
                padding: 10px 20px;
            }
            .button.translate{
                position: absolute;
                top: -3%;
                right: 65%;
                font-size: 20px;
            }
        }  
    }
</style>
