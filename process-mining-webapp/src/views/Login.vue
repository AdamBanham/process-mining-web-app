<template>
    <b-notification class="login" :closable="false">
        <div class="login-controls">
            <loginForm />
        </div>
        <div class="login-loading">
            <b-loading :active="true" :is-full-page="true" class="login-loading">
                    <p>
                    <b-icon
                        pack="fas"
                        icon="sync-alt"
                        size="is-large"
                        custom-class="fa-spin">
                    </b-icon>
                    </p>
                    <p>
                    Please login to continue
                    </p>
            </b-loading>
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
p
    color: snow;
    margin-left: 3%;
.login
    margin-top: 5vh;
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