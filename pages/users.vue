<template>
  <div>
    <input type="text" v-model="inputUserId" />
    <button @click="goToUser">go to user {{ inputUserId }}</button>
    <nuxt-child/>
  </div>
</template>
<script>
export default {
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