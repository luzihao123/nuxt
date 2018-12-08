<template>
  <div>
    <div class="diss">
      <!-- <img src="../static/logo_blue.png" alt=""> -->
      <img src="~static/logo_blue.png" alt="">
    </div>
    <ul>
      <li><nuxt-link :to="{name:'index'}">Home</nuxt-link></li>
      <li><nuxt-link :to="{name:'about'}">About</nuxt-link></li>
      <li><nuxt-link :to="{name:'news',params:{'id':330}}">News</nuxt-link></li>
      <li><nuxt-link :to="{name:'asyncData'}">Async</nuxt-link></li>
    </ul>
  </div>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
   
  }
}
</script>

<style>
  .diss{
    width:300px;
    height:100px;
    background-image: url('~static/logo_blue.png')
  }
</style>

