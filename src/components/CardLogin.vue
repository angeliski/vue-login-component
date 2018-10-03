<template>
  <section class="login_container">
      <div class="login_panel">
        <input class="form-element" v-model="email" placeholder="Email" type="email" >
        <input class="form-element" v-model="password" type="password" />
        <button @:click="login" class="form-element">Entrar</button>
      </div>
    </section>
</template>

<script>
export default {
  name: "CardLogin",
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
  }
};
</script>
// Mudar para CSS module
<style scoped>
.login_container {
  background-color: gray;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.login_panel {
  max-width: 50%;
  padding: 2.75rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: #fff;
  border-radius: .25rem;
  box-shadow: 1px 1px 5px 0px rgba(0,0,0,0.75);
}
.form-element {
    display: block;
    width: 100%;
    height: calc(2.25rem + 2px);
    padding: .3rem .7rem;
    font-size: 1rem;
    line-height: 1.5;
    color: #495057;
    background-clip: padding-box;
    border: 1px solid #ced4da;
    border-radius: .25rem;
    transition: border-color .15s ease-in-out,box-shadow .15s ease-in-out;
    margin-bottom: 1rem!important;
}
</style>
