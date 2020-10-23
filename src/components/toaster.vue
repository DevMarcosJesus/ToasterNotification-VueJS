<template>
  <div id="toaster">
     {{a}}
  </div>
</template>

<script>

import Vue from 'vue';
import VueToast from 'vue-toast-notification';
import 'vue-toast-notification/dist/theme-default.css';

Vue.use(VueToast);
Vue.$toast.success('Jesus The King', {
  position: 'top',
  duration: 3000,
})

Vue.$toast.default('123123',{
    position: 'bottom',
    duration: 2000,
})

export default {
    el: "#toaster",
    data(){
        return{
        a: 'socorro'
        }
    },
    
}
</script>

<style>
#toaster{
    margin-top: 100px;
}
</style>