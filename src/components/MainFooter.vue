<template>
    <v-footer
            absolute
            class="font-weight-medium mt-10">
        <v-flex xs12 md6>
            <strong>A Funush Private Limited Venture </strong> &copy; {{ new Date().getFullYear() }}
        </v-flex>
        <v-flex xs12 md6>
            <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn
                        text
                        style="color: #212121;"
                >
                    About Us
                </v-btn>

                <v-btn
                        text
                        style="color: #212121;"
                >
                    Contact Us
                </v-btn>
            </v-card-actions>
        </v-flex>
    </v-footer>
</template>
