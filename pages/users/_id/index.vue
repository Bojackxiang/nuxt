<template>
  <div>
    a sigle user  {{$route.params.id}}
  </div>
</template>

<script>
  export default {
    validate(data){
      console.log(data);
      // return data.params.id === 1
      console.log(data.params.id);
      return data.params.id === '1'
    }
  }
</script>

<style lang="scss" scoped>

</style>