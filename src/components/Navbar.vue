<template>
    <v-app-bar app dark style="background: #007799;" class="navbar">
        <img
                src="../assets/logo.png"
                alt="John"
        >
        <v-spacer></v-spacer>
        <v-toolbar-items style="color: #F0F0F0">
            <v-btn text style="border-right: 2px solid #335F9F" class="d-block">
                <ul>
                    <li><img src="../assets/connect_white.png" alt=""></li>
                    <li><span>Connect</span></li>
                </ul>
            </v-btn>
            <v-btn text style="border-right: 2px solid #335F9F">
                <ul>
                    <li><img src="../assets/Test_white.png" alt=""></li>
                    <li><span>Career Test</span></li>
                </ul>
            </v-btn>
            <v-btn text style="border-right: 2px solid #335F9F">
                <ul>
                    <li><img src="../assets/Opportunity.png" alt=""></li>
                    <li><span>Explore</span></li>
                </ul>
            </v-btn>
            <v-btn text style="border-right: 2px solid #335F9F">
                <ul>
                    <li><img src="../assets/speech-bubble-with-text-lines.png" alt=""></li>
                    <li><span> Message</span></li>
                </ul>
            </v-btn>
            <v-btn text>
                <ul>
                    <li><img src="../assets/notification.png" alt=""></li>
                    <li><span>Notification</span></li>
                </ul>
            </v-btn>
            <template v-if="$vuetify.breakpoint.smAndUp">
                <v-btn icon>
                    <v-avatar class="mr-2">
                        <img src="../assets/Profile_image.png" small alt="">
                    </v-avatar>
                    <img src="../assets/Dropdown.png" alt="">
                </v-btn>
            </template>
        </v-toolbar-items>
    </v-app-bar>
</template>
<style>
    @import url('https://fonts.googleapis.com/css?family=Poppins:400,400i,500,500i&display=swap');

    .navbar {
        font-family: 'Poppins', sans-serif;
        font-size: 12px;
        padding: 10px 0;
    }
    .navbar ul li {
        font-size: 12px;
    }
</style>
