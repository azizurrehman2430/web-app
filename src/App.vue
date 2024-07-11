<template>
  <v-app>
    <v-app-bar color="primary" >
      <!-- <span>
          <h2>
            Logo
          </h2>
        </span> -->
        <v-img :src="require('../src/assets/Logo.png')" id="image"  class="ml-0"  border-radius="50%"/>
       <v-spacer></v-spacer>
       <v-btn id="btn" to="/">Home</v-btn>|
      <v-btn class="btn" to="/about">About</v-btn>|
      <v-btn  class="btn" to="/Services">Services</v-btn>|
      <v-btn class="btn" to="/Contact">Contact Us</v-btn>
       
    </v-app-bar>
    <router-view/>
  </v-app>
  </template>
  
  
  <style>
  #image{
    width: 100px;
    height: 100px;
    margin-right:60rem;
  }
  #btn{
    margin-left: -100px;
  }
  </style>
  <script>
  export default {
    name: "App",
  };
  </script>
  