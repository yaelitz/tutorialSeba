<template>
  <v-container fluid>
    <v-slide-y-transition mode="out-in">
      <v-layout column>
       <v-card class="pa-4">
          <h2>¿En que flu fluf lfu?</h2>
          <v-layout wrap>
              <v-flex xs12 sm6>
                  ACA VA EL PICKER
              </v-flex>
              <v-flex xs12 sm6>
                  ACA VA EL PICKER
              </v-flex>
          </v-layout>
          <h2 class="pt-2">Agregar personas</h2>
          <v-layout class="pt-2">
              <v-flex xs2>
                <v-btn color="primary">Todos</v-btn>                  
              </v-flex>
              <v-flex xs3>
                <v-select
                :items="items"
                v-model="e1"
                label="Select"
                single-line
                autocomplete
                ></v-select>
                                        
              </v-flex>
              <v-flex xs4>
                <v-btn color="primary">Todos</v-btn>                  
              </v-flex>
              <v-flex xs3>
                <v-btn color="primary">Todos</v-btn>                  
              </v-flex>

          </v-layout>

       </v-card>
      </v-layout>
    </v-slide-y-transition>
  </v-container>
</template>
<script>
export default {
    data(){
        return{
            items:["fla", "fli", "flu"],
            e1:null
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
