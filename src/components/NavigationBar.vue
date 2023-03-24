<template>
  <div class="navbar">
    <img src="../assets/logo.svg" class="logo" />
 
    <ul>
      <li>Home</li>
      <li>New</li>
      <li>Popular</li>
      <li>Trending</li>
      <li>Categories</li>
    </ul>

    <img src="../assets/icon-menu.svg" class="mobile-menu"/>

    <div class="mobile-list" >
        <ul>
          <img src="../assets/icon-menu-close.svg" style="color: black; font-size: 2rem"/>
          <li>Home</li>
          <li>New</li>
          <li>Popular</li>
          <li>Trending</li>
          <li>Categories</li>
        </ul>
      </div>
  </div>
</template>

<style scoped>
.navbar {
  background-color: white;
  display: flex;
  justify-content: space-between;
  height: 15vh;
  align-items: center;
  color: grey;
  
  /* font-family:'Inter', sans-serif ; */
}
.navbar .logo{
  width: 6%;
  height: 35%;
  
}


.navbar ul {
  display: flex;
  list-style: none;
  margin-right: 15%;
  
}

.navbar ul li {
  font-family: "Inter", sans-serif;
  font-size: small;
  font-weight: 600;
  justify-content: space-between;
  margin-left: 15%;
}

.navbar ul li:hover {
  color: hsl(5, 85%, 63%);
}

.navbar .mobile-menu{
  display: none;
}
.navbar .mobile-list{
  display: none;
}



@media (max-width: 800px){
  .navbar{
    height:10vh ;
    background-color: white;
  }
  .navbar .logo{
    margin-left: 3%;
    width: 9%;
  }

  .navbar ul li{
    display: none;

  }
  .navbar .mobile-menu{
    display: flex;
    margin-right: 3%;
    
  height: 30%;
  }

   .navbar .mobile-list {
    display: flex;
    flex-direction: column;
    background-color: rgba(0, 0, 0, 0.5);
    min-height: 410%;
    position: absolute;
    width: 100vw;
    top: -100%;
    padding: 0;
    z-index: 500;
    margin: 0;
  }
   .navbar .mobile-list ul {
    flex-direction: column;
    margin-left:25%;
    background-color: white;
    justify-content: flex-start;
    width: 60vw;
    height: 350vh;
    padding-right: 6vw;
    padding-top: 10vh;
   
  }

 .navbar .mobile-list ul li {
    font-weight: 700;
    color: black;
    list-style: none;
    margin-bottom: 20%;
  }

}
</style>
