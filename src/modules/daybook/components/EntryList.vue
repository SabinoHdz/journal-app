<template>
  <h1>Entry List!!!</h1>
  <div class="entry-list-container">
    <div class="px-2 pt-2">
        <input type="text" name="search_entry" id="search_entry" class="form-control" placeholder="Buscar entrada">
    </div>
    <div class="entry-scrollarea">
        <EntryView v-for="item in 100" :key="item"/>
           
    </div>
  </div>
</template>

<script>
import { defineAsyncComponent } from "vue";
export default {
  components: { EntryView:defineAsyncComponent(()=>import('./EntryView.vue')) },

}
</script>

<style lang="scss" scoped>
.entry-list-container{
    border-right:1px solid #2c3e50;
    height:calc(100vh - 56px);
}
.entry-scrollarea{
    height: calc(100vh - 120px);
    overflow: scroll;
}
</style>