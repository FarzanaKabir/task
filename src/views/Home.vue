<template>
    <div class="home">
        <template>
            <v-container grid-list-md>
                <v-layout wrap>
                    <v-flex xs12 md4>
                        <sidebar></sidebar>
                    </v-flex>
                    <v-flex xs12 md8>
                        <main-content></main-content>
                    </v-flex>
                </v-layout>
            </v-container>
        </template>
    </div>
</template>

<script>
    import Sidebar from '../components/Sidebar'
    import MainContent from '../components/MainContent'

    export default {
        name: 'Home',
        // eslint-disable-next-line vue/no-unused-components
        components: {Sidebar, MainContent}
    };
</script>
