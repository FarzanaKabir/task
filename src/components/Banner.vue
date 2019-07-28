<template>
    <v-container fluid grid-list-md text-center class="px-0 mx-0">
        <img class="image" src="../assets/banner_image.png" alt="" width="100%" height="550px">

        <template>
            <v-container class="form" grid-list-md text-center>
                <v-layout wrap>
                    <v-flex
                            xs12
                            md9
                            d-flex
                    >
                        <v-select style="border-radius: 0"
                                  :items="items"
                                  label="Select Your Interest/Industry"
                                  outlined
                        ></v-select>

                    </v-flex>

                    <v-flex
                            xs12
                            md3
                    >
                        <v-btn class="btn" dark style="background: #007799">Get Started</v-btn>
                    </v-flex>
                </v-layout>
            </v-container>
        </template>
        <template>
            <v-container class="banner-text" text-center grid-list-md>
                <v-layout wrap>
                    <v-flex xsl12 md4 class="px-0">
                        <a href="#">Find Professonals</a>
                    </v-flex>
                    <v-flex xsl12 md4 class="px-0">
                        <a href="#">Get Connected</a>
                    </v-flex>
                    <v-flex xsl12 md4 class="px-0">
                        <a href="#">Increase Job Opportunities</a>
                    </v-flex>
                </v-layout>
            </v-container>

        </template>
    </v-container>
</template>
<script>
    export default {
        data: () => ({
            select: null,
            items: [
                'Industry 1',
                'Industry 2',
                'Industry 3',
                'Industry 4',
            ],
        }),
    }
</script>
<style>
    @import url('https://fonts.googleapis.com/css?family=Poppins:400,400i,500,500i&display=swap');

    .image {
        position: relative;
    }

    .form {
        position: absolute;
        top: 15%;
        right: 0;
        left: 0;
        width: 700px;
        height: 80px;
        margin: 0 auto;
        background: #fff;
    }

    .btn {
        height: 64% !important;
        border: none !important;
        -webkit-border-radius: 0;
        -moz-border-radius: 0;
        border-radius: 0;
    }

    .banner-text {
        font-family: 'Poppins', sans-serif;
        position: absolute;
        top: 22%;
        color: #F0F0F0;
    }

    .banner-text a {
        color: #F0F0F0 !important;
        font-size: 22px;
        text-decoration: none;
        padding: 0;
    }

    .banner-text a:after {
        position: absolute;
        content: '';
        background: #93EE0B;
        -webkit-border-radius: 50%;
        -moz-border-radius: 50%;
        border-radius: 50%;
        width: 7px;
        height: 7px;
        transform: translate(3px, 17px);

    }
</style>
