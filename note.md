### 获取 route param
```vue  
<template>
  <div>
    a sigle user  {{$route.params.id}}
  </div>
</template>
```

### 导航的的两种方法
第一种
```vue  
<template>
  <nuxt-link to="/users">Users</nuxt-link>
</template>
```
第二种
```javascript
methods:{
  goToUser(){
    this.$router.push(`users/${this.inputUserId}`)  
  }
}
```


