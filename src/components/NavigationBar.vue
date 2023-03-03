<template>
  <div class="navbar">
   
   <img  src="../assets/logo.svg"/>
    <ul>
        <li>Home</li>
        <li>New</li>
        <li>Popular</li>
        <li>Trending</li>
        <li>Categories</li>
    </ul>

  </div>

</template>

<script setup>


</script>

<style>

.navbar{
    background-color: white;
    display: flex;  
    justify-content: space-around;
    height: 100px;
    gap: 20%;
    max-width: 1200px;
    align-items: center;
}
.navbar img{
  width: 70px;
  height: 45px;
  margin-left: -200px;
}

.navbar ul{
  display: flex;
  list-style: none;
  gap: 20%;
  

 
}





</style>