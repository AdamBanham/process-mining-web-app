<template>
  <div class="login-form">
      <b-field label="Username" class="login-field">
          <b-input v-model="username" />
      </b-field>
      <b-field label="Password" class="login-field">
          <b-input v-model="password" />
      </b-field>
      <b-button @click="login" class='is-info login-button'>Login</b-button>
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
    z-index: 30;
    position: relative;
.login-button
    width: 150px;
.login-field
    margin-left: 3%;
    margin-right: 3%;

</style>