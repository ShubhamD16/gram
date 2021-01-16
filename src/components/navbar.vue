<template>
  <nav>
    <v-app-bar flat app class="grey lighten-3">
      <v-app-bar-nav-icon v-on:click.prevent="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title class="grey--text ">
        <span class="font-bold-light text-uppercase " >Gram</span>
        <span class="font-weight-light text-uppercase " > Seva</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn  class="hidden-md-and-up" plain color="grey darken-3" >
        <v-icon left>exit_to_app</v-icon>
        <span >woo</span>
      </v-btn>
       <v-btn plain color="grey darken-3"> 
        <span>woohoo</span>
      </v-btn>
      
    </v-app-bar>
    <v-navigation-drawer v-model='drawer' app>
      <v-system-bar></v-system-bar>
      <v-list>
        <v-list-item v-for="item in draweritem" v-bind:key=item.title router :to="item.route">
          <v-list-item-icon>
            <v-icon>{{item.icon}}</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>
              woohooowooohooo
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  data(){
    return{
      drawer:false, 
      draweritem:[
        {"title":"t1","icon":"dashboard","route":"/"},
        {"title":"t2","icon":"error","route":"/kq"},
        {"title":"t3","icon":"mail","route":"/kk"},
      ]
    }
  }

}
</script>

<style>

</style>