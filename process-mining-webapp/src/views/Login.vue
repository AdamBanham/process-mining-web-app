<template>
    <div class="login-view">
        <b-notification class="login" :closable="false">
            <div class="login-controls">
                <loginForm />
            </div>
        </b-notification>
        <div class="login-loading">
                <b-loading :active="true" :is-full-page="true">
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
    </div>
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
$break-medium: 1000px;
$loading-background: rgba(255,255,255,0.7) !important;
p
    color: snow;
    margin-left: 3%;
.login
    margin-top: 5vh;
    max-width: 35vw;
    max-height: 30vh;
    margin-left: 32.5vw;
    padding: 2em;
    @media screen and (max-width: $break-medium)
        max-width: 50vw;
        margin-left: 25vw;
    @media screen and (max-width: $break-small)
        max-width: 80vw;
        margin-left: 10vw;
.login-loading
    z-index: 29;
    position: relative;
</style>