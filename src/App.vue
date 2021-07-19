<template>
  <v-app>
    <v-app-bar
      flat
      dense
      class="nav"
      color="white"
      height="20vh"
      
    >
      Menu Bar
    </v-app-bar>

    <!-- Navigation Drawer -->
    <v-row class="main-row"  no-gutters>
      <v-col  cols="2">
        <p class="text-h3 font-weight-bold">Side Bar </p>
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
.nav{
  font-family: 'Source Sans Pro', sans-serif;
}
.rounded-left{
  border-top-left-radius: 15px;
  overflow-y: scroll;
  height: 100%;
  background-color: #ECF4F7;
 

}
.main-row{
  height:80vh;
  font-family: 'Source Sans Pro', sans-serif;
}
::-webkit-scrollbar {
    display: none;
    }


</style>
