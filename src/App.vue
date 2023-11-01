<template>
 <notebooks-panel :cards-list-data="notebooksList"/>
</template>

<script>
import NotebooksPanel from "./components/NotebooksPanel.vue";
import { notebooksList} from "./constants/3_data_notebooks";


export default{
  name:'App',

  components:{
   NotebooksPanel,
  },

  data(){
    return{
      notebooksList

  }}

}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

