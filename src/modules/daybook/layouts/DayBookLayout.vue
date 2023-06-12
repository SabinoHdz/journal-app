<template>
  <NavbarView/>
  <div class="d-flex">
    <div class="col-4">
      <entry-list></entry-list>
    </div>
    <div class="col">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'
import EntryList from '../components/EntryList.vue'
export default {
components:{
    NavbarView:defineAsyncComponent(()=>import('../components/NavbarView.vue')),
    EntryList
}
}
</script>
<style>

</style>