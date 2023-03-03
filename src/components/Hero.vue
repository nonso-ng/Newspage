<template>
    <div class="hero">
        <div class="hero-left">
            <div class="hero-left-top"></div>
            <div class="hero-left-bottom">
                <div class="hero-left-bottom-left">
                    <h1>The Bright Future Of Web 3.0?</h1>
                </div>

                <div class="hero-left-bottom-right">
                    <div>left bottom right</div>
                    <button class="btn">READ MORE</button>
                </div>

            </div>
        </div>
        <div class="hero-right"> part 2</div>
    </div>
</template>


<style>

  

.hero{
    background-color: white;
    display: grid;
    gap: 20px;
    height:62vh;
    grid-template-columns: 2fr 1fr;
    
    font-family: 'Inter', sans-serif;
}
.hero-right{

}
.hero-right{
    background-color: hsl(240, 100%, 5%);
}
.hero-left-top{
    
    background-image: url(../assets/image-web-3-desktop.jpg);
    background-size: cover;
    height: 40vh;
}
.hero-left-bottom{
    display: grid;
    grid-auto-flow: column;
    grid-template-columns: 1fr 1fr;
    
    
}
.hero-left-bottom-left{
background-color: coral;
font-size: 23px;
font-weight: bolder;

}
.hero-left-bottom-right{
    background-color: darkred;
    
}

.btn{
    background-color: hsl(35, 77%, 62%);
    color: white;
    
}

</style>