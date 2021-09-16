<template>
<div class="app">
<header><h1>SearchVue</h1>


    <nav>
      <a href="">Characters</a>
      <a href="">Persons</a>
      <div class="box">
      </div>
  
      <a class="menu" href="">Menu</a>
    </nav>
  </header>
  <main><h2>Search for your favourite Star Wars character or planet!</h2>
  <div class="container">
   <div class="search-box">
      <input type="text" class="search-input" placeholder="Search..">

      <button class="search-button">
        <i class="fas fa-search"></i>
      </button>
   </div>
</div>
  <ul>
    <li class="Persons">Persons</li>
  </ul>
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
  height: 100vh;
  text-align: center;
  background-color:black;
}
/*Flex items*/
header {
  background-color:rgb(165, 207, 221);
  flex-grow: 1;
}
.box{
flex-grow: 2;
flex-direction: row;
margin: 1em;

}
main{
  background-color:lightgrey;
  flex-grow: 2;
}

footer{
  background-color:grey;
  flex-grow: 1;
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
  border: 4px solid #111d5e;
  border-radius:10px 0 0 10px ;
  border-right: none;
  outline: none;
  font-size: 20px;
  color: tomato;
  background: none;
}
.search-button{
 text-align: center;
height: 51px;
width: 40px;
outline: none;
cursor: pointer;
border: 4px solid #111d5e;
 border-radius: 0 10px 10px 0 ;
border-left: none;
background: none;
font-size: 20px;
border-left: 4px solid #111d5e;


}
.container{
  width: 35%;
  position: absolute;
  left: 50%;
  top: 40%;
  transform: translate(-50% , -50%);
}

</style>
