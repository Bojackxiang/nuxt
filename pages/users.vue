<template>
  <div>
    <input type="text" v-model="inputUserId" />
    <button @click="goToUser">go to user {{ inputUserId }}</button>
    <NuxtChild />
  </div>
</template>
<script>
export default {
  layout: 'users',
  data() {
    return {
      inputUserId: "",
    };
  },
  methods: {
    goToUser() {
      // this.$router.push(`users/${this.inputUserId}`);

      console.log('this.router.params: ', this.$router.push(`users/${this.inputUserId}`));

    },
  },
};
</script>

<style lang="scss" scoped>
</style>