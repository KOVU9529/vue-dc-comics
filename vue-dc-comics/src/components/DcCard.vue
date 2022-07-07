<template>
    <div class="dc-card">
        <img :src="dcDetails.thumb" :alt="dcDetails.series">
        <h2>{{dcDetails.series}}</h2>
    </div>
</template>

<script>
export default {
    name:'DcCard',
    props:{
        dcDetails: Object
    }
}
</script>

<style lang="scss" scoped>
    .dc-card{
        background-color:#1c1c1c ;
        width: calc((100% / 6) - 8px);
        margin:4px;
        img{
            object-fit: cover;
            object-position: top;
            width: 100%;
            height: 60%;
        }
        h2{
            color: white;
            font-size: 10px;
        }
    }
</style>