<template>
<div class="app">
<header><h1>SearchVue</h1>

  </header>
  <main><h2>Search for your favourite Star Wars characters or movies!</h2>
  <div class="container">
   <div class="search-box">
      <input type="text" class="search-input" placeholder="Search..">

      <button class="search-button">
        <i class="fas fa-search"></i>
      </button>
   </div>
</div>
<div class="Boxes">
  <ul>
    <li class="Characters"><h3>Characters</h3></li>
    <li class="Movies"><h3>Movies</h3></li>
  
  </ul>
</div>
  </main>


  <footer><h3>About Us!</h3>
  
  </footer>
  
</div>

</template>

<script>
export default {}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /*margin-top: 60px;*/
  
}
  *{padding: 0px; margin: 0px;}
.app {
    display: flex;
    flex-direction: column;
    height: 100vh;
}
body{
  /*flex container */
  background-image: url("https://cdn.pixabay.com/photo/2016/01/27/15/25/space-1164579_960_720.png");
 background-color: #cccccc;
  height: 100vh;
  text-align: center;
  /*background-color:black;*/
  
}
/*Flex items*/
header {
  /*background-color:rgb(165, 207, 221);*/
  color: yellow;
  flex-grow: 1;
  max-height: 100px;
  
}
.box{
flex-grow: 2;
flex-direction: row;
margin: 1em;

}
main{
  /*background-color:lightgrey;*/
  background-image: url("https://cdn.pixabay.com/photo/2016/01/27/15/25/space-1164579_960_720.png");
 background-color: #cccccc;
 color: yellow;
  flex-grow: 2;
}

footer{
  /*background-color:grey;*/
  color: yellow;
  flex-grow: 1;
  max-height: 100px;
}
nav {
  display: flex;
  flex-direction: row;
  
}
nav .menu{
float: right;
position: relative;

}
nav a {
  border: 1px solid gray;
  margin: 0.3em;
  padding: 0.5em 2em;
  background-color: white;
  border-radius: 2em;
  
}
.search-box{
  width: 100%;
  position: relative;
  display: flex;

}
.search-input{
  width: 100%;
  padding: 10px;
  border: 4px solid yellow;
  border-radius:10px 0 0 10px ;
  border-right: none;
  outline: none;
  font-size: 20px;
  color:yellow;
  background: none;
}
.search-button{
 text-align: center;
height: 51px;
width: 40px;
outline: none;
cursor: pointer;
border: 4px solid yellow;
 border-radius: 0 10px 10px 0 ;
border-left: none;
background: none;
font-size: 20px;
border-left: 4px solid yellow;


}
.container{
  width: 35%;
  position: relative;
  left: 50%;
  transform: translate(-50% , -50%);
  margin-top: 35px;
}

.boxes li {
display: flex;
}

</style>
