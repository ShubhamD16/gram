<template>
  <div>
    <v-container ma-1 fluid>
      <v-row >
        <v-col class="d-flex justify-center" cols="12" md="4" sm="6" v-for="n in 5"  :key="n">
         <v-card class="d-flex  justify-center " max-width="300">
           <v-card-title primary-title>
             <div>
               <h2 class=" h2 mb-1  text-center">Village name</h2>
               <h3 class="subtitle-1  text-center">Village name</h3>
               <hr>
               <div>total-records:178</div>
               <div>valadity:180 days</div>
               <v-card-actions class="d-flex justify-center">
                <v-btn color="success " @click="details(name)">view</v-btn>
               </v-card-actions>    
             </div>
           </v-card-title>
          
         </v-card>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid grid-list-xs>
      <hr>
      <v-card flat class="d-flex justify-center">
        <v-card-title class="d-block text-center" primary-title>
          title
          <h3 class="d-block text-center" >kldsjdslk</h3>

        </v-card-title>
        
      </v-card>
      
    </v-container>
    
  </div>
</template>

<script>
export default {
  data(){
    return{
      name:'warangi',
    };
  },

methods:{
  details(id){
    this.$router.push({name:'Home'})
    console.log(id);
  }
}
}
</script>

<style>

</style>