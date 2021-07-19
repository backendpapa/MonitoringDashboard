<template>
  <v-app>
    <v-app-bar
      flat
      dense
      color="white"
      height="20vh"
      
    >
      Menu Bar
    </v-app-bar>

    <!-- Navigation Drawer -->
    <v-row class="main-row"  no-gutters>
      <v-col  cols="2">
        Side Bar 
      </v-col>
      <v-col cols="10" class="rounded-left">

        <v-main style="padding:3rem">
           <router-view/>
        </v-main>
   
      </v-col>
    </v-row>

    


    
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
<style>
.rounded-left{
  border-top-left-radius: 15px;
  overflow-y: scroll;
  height: 100%;
  background-color: #ECF4F7;

}
.main-row{
  height:80vh
}
::-webkit-scrollbar {
    display: none;
    }


</style>
