<template>
    <v-app>
        <navbar></navbar>
        <banner></banner>
        <v-content>
            <v-container fluid>
                <router-view></router-view>
            </v-container>
        </v-content>
        <main-footer></main-footer>
    </v-app>
</template>

<script>
    import Navbar from './components/Navbar'
    import Banner from './components/Banner'
    import MainFooter from './components/MainFooter'

    export default {
        name: 'App',
        // eslint-disable-next-line vue/no-unused-components
        components: {Navbar, Banner, MainFooter},
        data: () => ({
            //
        }),
    };
</script>

<style>
    body {
        font-family: 'Poppins', sans-serif;
    }
</style>
