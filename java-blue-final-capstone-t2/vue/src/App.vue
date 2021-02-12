<template>
  <div id="app">
    <div id="nav">
      
      <router-link v-bind:to="{ name: 'home' }" v-if="$store.state.token != ''"><button class = "home-button">Home</button></router-link> &nbsp;&nbsp;
      <router-link v-bind:to="{name: 'matched'}" v-if="$store.state.token != ''"><button class = "liked-button">Liked Restaurants</button></router-link>&nbsp;&nbsp;
      <router-link v-bind:to="{ name: 'logout' }" v-if="$store.state.token != ''"><button class = "logout-button">Logout</button></router-link> 
      
    </div>
    <router-view />
  </div>
</template>

<style>
@import './assets/Main.css';


.logout-button {
  background-color: #AFEADC;
  border-color: #041E42;
  border-radius: 5px;
  height: 25px;
  width: 75px;
  font-family: Quicksand;
  font-weight: bold;
  text-transform: uppercase;
}

.liked-button {
  background-color: #AFEADC;
  border-color: #041E42;
  border-radius: 5px;
  height: 25px;
  width: 155px;
  font-family: Quicksand;
  font-weight: bold;
  text-transform: uppercase;
}

.home-button {
  background-color: #AFEADC;
  border-color: #041E42;
  border-radius: 5px;
  height: 25px;
  width: 75px;
  font-family: Quicksand;
  font-weight: bold;
  text-transform: uppercase;
}


</style>
