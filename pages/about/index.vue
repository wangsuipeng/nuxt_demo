<template>
  <div>
      <nuxt/>
      <h2>About Index page</h2>
      <ul>
        <!-- <li><a href="/">Home</a></li> -->
        <li><nuxt-link :to="{name: 'index'}">Home</nuxt-link></li>
      </ul>
  </div>
</template>
<script>
export default {
    transition:'test'
}
</script>
