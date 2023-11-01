
<template>
    <a class='card' :href='cardData.link'>
        <div class="image"><img :src="cardData.imgSrc"></div>
        <div class="block">
        <div class="info-block">
            <div class="title">{{cardData.title}}</div>
             <div class="discount">Ваша економiя <span>{{cardData.discount}}₴</span></div>
        </div>
        <div class="price-block">
           <div class="price-items">
                <div class="old-price"> {{cardData.oldPrice}}₴</div>
                <div class="current-price"> {{cardData.price}}₴</div>
           </div>
            <div><button class="button">Купити</button></div>
        </div>
        </div>
    </a>
</template>

<script>
    export default {
        name:'NotebookCard',

        props:{
            cardData:{
                type:Object,
                default:()=>({})
            }
        }
    }
</script>

<style lang="css" scoped>
.card {
    color: #000000;
    text-decoration: none;
    margin-bottom: 30px;
    gap: 30px;
    width:800px;
    display: flex;
    }
.title{
   font-size: 20px;
   color: rgb(71, 141, 211);
   font-weight: 700;
   margin-bottom: 10px;

}
.image img{
    max-width: 200px;
     border-radius: 10px;
}

.price-block{
    display: flex;
    justify-content: space-between;
    
}
.discount{
    font-weight: 700;
    font-size: 14px;
    color: rgb(88, 88, 88);
}
.discount span{
color:red;
}
.info-block{
    margin-bottom: 20px;
}
.current-price{
    font-size: 20px;
    color: red;
}
.old-price{
    font-size: 16px;
    color: rgb(137, 137, 137);
    text-decoration: line-through;
}
.price-items{
   
}
.block{
    flex: 0 1 700px;
}
.button{
    background: #00a046;
    border: none;
    color: #ffffff;
    cursor: pointer;
    border-radius: 12px;
    padding: 10px 20px;
}
		



</style>