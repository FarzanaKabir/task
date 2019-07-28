<template>
    <div class="sidebar">
        <template>
            <v-card style="border: 1px solid #00A8D8" class="sidebar-card">

                <v-toolbar style="background: #007799; height: 125px; padding: 25px 0;" text-center align-center>
                    <v-card-text style="color: #F0F0F0; text-align: center;">
                        <h2 style="color: #93EE0B">Industry: Technology</h2>
                        <h3 style="padding: 12px 0">Average Entry Lavel Salary</h3>
                        <h1>25000 BDT</h1>
                    </v-card-text>
                </v-toolbar>

                <v-card-text style="text-align: left">
                    <v-list flat>
                        <v-list-item-group v-model="item" color="primary">
                            <v-list-item>
                                <h2 style="color: #212121;">Popular Careers In July 2019</h2>
                            </v-list-item>
                            <v-list-item
                                    v-for="(item, i) in items"
                                    :key="i"
                            >

                                <v-list-item-content>
                                    <v-list-item-title v-text="item.text"></v-list-item-title>
                                </v-list-item-content>
                            </v-list-item>
                        </v-list-item-group>
                    </v-list>
                </v-card-text>

                <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn
                            text
                            color="Black"
                    >
                        SEE MORE
                    </v-btn>


                </v-card-actions>
            </v-card>
        </template>
    </div>
</template>
<script>
    export default {
        data: () => ({
            item: 1,
            items: [
                {text: 'Product Development'},
                {text: 'UI/UX Design'},
                {text: 'App Development'},
                {text: 'Cloud Server Management'},
                {text: 'Data Analyst'},
                {text: 'Usability Analyst'},
            ],
        }),
    }
</script>
<style>
    @import url('https://fonts.googleapis.com/css?family=Poppins:400,400i,500,500i&display=swap');
    .sidebar{
        font-family: 'Poppins', sans-serif;
    }
    .sidebar .sidebar-card {
        box-shadow: none;
        border-radius: 0;
    }

</style>
