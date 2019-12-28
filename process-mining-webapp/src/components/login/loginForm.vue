<template>
  <div class="login-form">
      <b-field label="Username" class="login-field">
          <b-input v-model="username" />
      </b-field>
      <b-field label="Password" class="login-field">
          <b-input v-model="password" />
      </b-field>
      <div class="login-button">
        <b-button @click="login" class='is-info login-button-control'>Login</b-button>
      </div>
  </div>
</template>

<script>
export default {
    name: "loginForm",
    components: {

    },
    data() {
        return {
            password : null,
            username : null,
        }
    },
    methods : {
        login: function() {

        }
    }
}
</script>

<style lang="sass" scoped>
.login-form
    position: relative;
    z-index: 30;
    padding: 1%;
    margin-left: auto;
    margin-right: auto;
.login-button
    width: 150px;
    float: right;
    margin-right: 1em;
    .login-button-control
        width: 100%;
.login-field
    margin-left: 3%;
    margin-right: 3%;

</style>