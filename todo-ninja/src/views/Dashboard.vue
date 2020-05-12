<template>
  <div class="dashboard">
    <h1 class="subheading grey--text">Dashboard</h1>
    
    <v-container class="my-5">
      
      <v-row>
        <v-col cols="12" md="6">
          <v-btn outline block class="primary">1</v-btn>
        </v-col>
        <v-col cols="12" md="2">
          <v-btn outline block class="primary">2</v-btn>
        </v-col>   
        <v-col cols="12" md="2">
          <v-btn outline block class="primary">2</v-btn>
        </v-col>   
        <v-col cols="12" md="2">
          <v-btn outline block class="primary">2</v-btn>
        </v-col>                              
      </v-row>

      <v-row class="mb-6" no-gutters>
        <v-col cols="12" md="6">
          <v-card class="pa-2" outlined tile>1</v-card>
        </v-col>
        <v-col cols="12" md="2">
          <v-card class="pa-2" outlined tile>2</v-card>
        </v-col>   
        <v-col cols="12" md="2">
          <v-card class="pa-2" outlined tile>2</v-card>
        </v-col>   
        <v-col cols="12" md="2">
          <v-card class="pa-2" outlined tile>2</v-card>
        </v-col>                              
      </v-row>      

      <v-row class="mb-6" no-gutters>
        <v-col cols="6" md="3">
          <v-card class="pa-2" outlined tile>1</v-card>
        </v-col>
        <v-col cols="2" md="3">
          <v-card class="pa-2" outlined tile>2</v-card>
        </v-col>   
        <v-col cols="2" md="3">
          <v-card class="pa-2" outlined tile>2</v-card>
        </v-col>   
        <v-col cols="2" md="3">
          <v-card class="pa-2" outlined tile>2</v-card>
        </v-col>                              
      </v-row>        

      <v-row>
        <v-col cols="4" md="3">
          <v-btn outline block class="success">1</v-btn>
        </v-col>
        <v-col cols="4" md="3">
          <v-btn outline block class="success">2</v-btn>
        </v-col>        
      </v-row>

    </v-container>


  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Dashboard',
  components: {

  }
}
</script>
