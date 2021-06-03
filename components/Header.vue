<template>
  <div class="header-wrapper">
    <ul>
      <li class="header-item">
        <nuxt-link to="/users">users</nuxt-link>
        <nuxt-link to="/users/1">users_1</nuxt-link>
        <nuxt-link to="/">home</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style  scoped>
  .header-wrapper{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .header-item{
    list-style: none;
    min-width: 100px;
    text-align: center;
  }
</style>