<template>
  <div class="dashboard">
    <h1 class="subheading grey--text">Dashboard</h1>
    
  <v-container class="my-5">
    <v-card flat class="px-3">
      <v-row>
        <v-col cols="12" md="6">
          <div class="caption grey--text">Project Title</div>
          <div>Create a new website</div>
        </v-col>
        <v-col>
          <div class="caption grey--text">Person</div>
          <div>The Net Ninja</div>
        </v-col>
        <v-col>
          <div class="caption grey--text">Due Date</div>
          <div>1st Jan 2021</div>
        </v-col>
        <v-col>
          <div class="caption grey--text">Status</div>
          <div>ongoing</div>
        </v-col>
      </v-row>
  </v-card>
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
