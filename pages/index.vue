<template>
  <div>
    <ul>
      <!-- <li><a href="/">HOME</a></li> -->
      <li><nuxt-link :to="{name: 'index'}">HOME</nuxt-link></li>
      <li><nuxt-link :to="{name: 'ansyData'}">ASYNC</nuxt-link></li>
      <li><nuxt-link :to="{name: 'about'}">ABOUT</nuxt-link></li>
      <li><nuxt-link :to="{name: 'news',params:{newsId:3306}}">NEWS</nuxt-link></li>
      <!-- <li><a href="/about">ABOUT</a></li>
      <li><a href="/news">NEWS</a></li> -->
    </ul>
  </div>
</template>
 
<script>
 
export default {
  components: {
   
  }
}
</script>
 
<style>
 
</style>