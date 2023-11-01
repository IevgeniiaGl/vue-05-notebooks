<template>
    <div class='panel'>
<notebook-card v-for="card in cardsListData" 
                :key="card.id"
                :card-data="card" 
            />
    </div>
</template>

<script>
import NotebookCard from './NotebookCard.vue'




    export default {
        name:'NotebooksPanel',
        components:{  NotebookCard},
        props:{
            cardsListData:{
            type:Array,
            default:() => [],
            }
        }
    }
</script>

<style lang="css" scoped>
.panel{
  
}
   

</style>