<template>
  <card-login />
</template>

<script>
import CardLogin from './CardLogin';
export default {
  name: "HelloWorld",
  data() {
    return {
      email: "",
     password: "" 
    };
  },
  methods: {
    login() {
      //TODO do login
    }
  },
  components: {
    CardLogin
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
