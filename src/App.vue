<template>
  <div id="App">
   <main>
     <div class="search-box">
       <input type="text" class="search-bar" placeholder="search"/>
     </div>
     <div class="weather-wrap">
       <div class="location-box">
         <div class="location">America, USA</div>
         <div class="date">Monday 20 January, 2024</div>
       </div>
 
       <div class="weather-box">
         <div class="temp">9* C</div>
         <div class="weather">Rain</div>
       </div>
     </div>
   </main>
  </div>
 </template>
 
 <script>
 
 
 export default {
   name: 'App',
  data () {
   return {
     api_key: 'aef35ae9b47f9137a211997acd1a4edf'
 
   }
  }
 }
 </script>
 
 <style>
 *{
   margin: 0;
   padding: 0;
   box-sizing: border-box;
 }
 #app {
   font-family: Avenir, Helvetica, Arial, sans-serif;
   -webkit-font-smoothing: antialiased;
   -moz-osx-font-smoothing: grayscale;
  
   background-image: url('./assets/cold-bg.jpg');
   background-size: cover;
   background-position: bottom;
 }
 
 main{
   min-height: 100vh;
   padding: 25px;
   background-image: linear-gradient(to bottom, rgba(0,0,0,0.25), rgba(0,0,0,0.75));
 }
 .search-box{
   width: 100%;
   margin-bottom: 30px;
 }
 
 .search-box .search-bar{
   display: block;
   width: 100%;
   padding: 15px;
   color: #313131;
   font-size: 20px;
   appearance: none;
   border: none;
   outline: none;
   box-shadow: 0px 0px 8px rgba(0,0,0,0.25);
   background-color: rgba(255,255,255,0.5);
   border-radius: 0px 16px 0px 16px;
   transition: 0.4s;
 }
 
 .search-box .search-bar:focus{
   box-shadow: 0px 0px 16px rgba(0,0,0,0.25);
   background-color: rgba(255,255,255,0.75);
   border-radius: 16px 0px 16px 0px;
 }
 
 .location-box .location{
   color: #FFF;
   font-size: 32px;
   font-weight: 500;
   text-align: center;
   text-shadow: 1px 3px rgba(0,0,0,0.25);
 }
 </style>
 