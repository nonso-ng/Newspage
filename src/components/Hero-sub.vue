<template>
    <div class="footer">
        <div class="part-one">
            <div class="part-one-img"></div>
            <div>jjjjjjjjjjjjjjjjjjjjj</div>
        </div>
        <div class="part-two">
            <div class="part-two-img"></div>
            <div></div>
        </div>
        <div class="part-three">
            <div class="part-three-img"></div>
            <div></div>
        </div>
    </div>
</template>

<style>
.footer{
    background-color: white;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    margin-top: 20px;
    gap: 9px;
}
.part-one{
 background-color: brown;
 display: grid;
 grid-auto-flow: column;
 grid-template-columns: 1fr 2fr;
 
}

.part-two{
    background-color:aquamarine ;
    display: grid;
    grid-auto-flow: column;
    grid-template-columns: 1fr 2fr;
}
.part-three{
    background-color: greenyellow;
    display: grid;
    grid-auto-flow: column;
    grid-template-columns: 1fr 2fr;
}

.part-one-img{
    background-image: url(../assets/image-retro-pcs.jpg);
    background-size: cover;
    
    height: 150px;
    width: 100%;

}
.part-two-img{
    background-image: url(../assets/image-top-laptops.jpg);
    background-size: cover;
    
    height: 150px;
    width: 100%;
}
.part-three-img{
    background-image: url(../assets/image-gaming-growth.jpg);
    background-size: cover;
    
    height: 150px;
    width: 100%;
}



</style>