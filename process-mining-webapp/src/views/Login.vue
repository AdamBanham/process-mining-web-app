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
$break-small: 600px;
.login
    max-width: 50vw;
    max-height: 30vh;
    margin-left: 25vw;
    padding: 3%
    @media screen and (max-width: $break-small)
        max-width: 80vw;
        margin-left: 10vw;
.login-loading
    z-index: 29;
    position: relative;
</style>