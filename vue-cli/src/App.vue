<template>
  <div>
    <app-header v-bind:propsdata="str" 
    v-on:eventRenew="parentPass"></app-header>
  </div>
</template>

<script>
import  AppHeader from './components/AppHeader.vue'
export default {
  data:function(){
    return{
      str:'Header'
    }
  },
  components:{
    'app-header':AppHeader
  },
  methods:{
    parentPass:function(){
      this.str = "clicked Send button";
    }
  }
}
</script>

<style>

</style>template