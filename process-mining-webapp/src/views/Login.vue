<template>
    <b-notification class="login" :closable="false">
        <div class="login-controls">
            <loginForm />
        </div>
        <div class="login-loading">
            <b-loading :active="true" :is-full-page="true" class="login-loading"></b-loading>
        </div>
    </b-notification>
</template>

<script>
import loginForm from '../components/login/loginForm'
export default {
    name:"login",
    components: {
        loginForm
    },

}
</script>

<style lang="sass" scoped>
.login
    width: 40vw;
    height: 30vh;
    margin-left: 30vw;
    padding: 3%
.login-loading
    z-index: 29;
    position: relative;
</style>