<template>
   <nav>
        <v-toolbar app>
            <v-toolbar-side-icon class="grey--text" @click="mini = !mini"></v-toolbar-side-icon>
            <v-toolbar-title class="text-upercase grey--text">
                <span class="font-weight-light">Dung</span>
                <span>bv</span>
            </v-toolbar-title>
            <v-spacer></v-spacer>
             <v-btn color="grey" flat>
                <span>Sign out</span>
                <v-icon right>exit_to_app</v-icon>
            </v-btn>
        </v-toolbar>
        <v-navigation-drawer app v-model="drawer" stateless  :mini-variant.sync="mini">
            <v-list>
                <v-list-tile router to="/">
                    <v-list-tile-action>
                        <v-icon>home</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                        <v-list-tile-title>
                            DasBroash
                        </v-list-tile-title>
                    </v-list-tile-content>
                </v-list-tile>
                <v-list-tile router to="/about">
                    <v-list-tile-action>
                        <v-icon>folder</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                        <v-list-tile-title>
                            About
                        </v-list-tile-title>
                    </v-list-tile-content>
                </v-list-tile>
            </v-list>
        </v-navigation-drawer>
   </nav>
</template>

<script>
    export default {
        data(){
            return {
                drawer:true,
                mini:false
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>