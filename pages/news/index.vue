<template>
  <div>
      <h2>News Index page</h2>
      <h1>{{$route.params.newsId}}</h1>
       <ul>
           <li><nuxt-link :to="{name: 'index'}">Home</nuxt-link></li>
           <li><nuxt-link :to="{name: 'news-id',params: {id: 456,title: '88888888888888'}}">News-1</nuxt-link></li>
           <li><nuxt-link :to="{name: 'news-id',params: {id: 123}}">News-2</nuxt-link></li>
        <!-- <li><a href="/">Home</a></li>
        <li><a href="/news/123">News-1</a></li>
        <li><a href="/news/456">News-2</a></li> -->
      </ul>
  </div>
</template>