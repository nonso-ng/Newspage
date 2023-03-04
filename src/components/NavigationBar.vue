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

<style scoped>


.navbar{
    background-color: white;
    display: flex;  
    justify-content: space-around;
    height: 100px;
    gap: 20%;
    max-width: 1200px;
    align-items: center;
    color: grey;
    /* font-family:'Inter', sans-serif ; */
    
    
   
}
.navbar img{
  width: 65px;
  height: 40px;
  margin-left: -200px;
}

.navbar ul{
  display: flex;
  list-style: none;
  gap: 20%;
  
}

.navbar ul li{
  font-family: 'Inter', sans-serif;
  font-size:small;
  font-weight: 520;
}

.navbar ul li:hover{
  color:hsl(5, 85%, 63%) ;
}





</style>