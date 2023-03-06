<template>
    <div class="hero">
        <div class="hero-left">
            <div class="hero-left-top"></div>
            <div class="hero-left-bottom">
                <div class="hero-left-bottom-left">
                    <h1>The Bright Future Of Web 3.0?</h1>
                </div>

                <div class="hero-left-bottom-right">
                    <p>We dive into the next evolution of the web that claims to put the hplatforms back into the hands of the people. But is it really fulfilling its promise?</p>
                    <button class="btn">READ MORE</button>
                </div>

            </div>
        </div>
        <div class="hero-right"> 
            <h1 style="color: hsl(35, 77%, 62%);">New</h1>
            <h3>Hydrogen VS Electric Cars</h3>
            <p>Will hydrogen fueled cars ever actch up to EVs?</p>
            <hr/>

            <h3>The Downsides of AI artistry</h3>
            <p>What are the possible on demand effect of on-demand AI image generation?</p>
            <hr/>

            <h3>Is VC funding drying up?</h3>
            <p>Private funding by VC firms is down 50% YOY, Wtake a look at what that means</p>
            
        </div>
    </div>
</template>


<style scoped>

  

.hero{
    background-color: white;
    display: grid;
    gap: 15px;
    height:67vh;
    grid-template-columns: 2.1fr 0.9fr;
    
    font-family: 'Inter', sans-serif;
}

.hero-right{
    background-color: hsl(240, 100%, 5%);
    color: white;
    padding: 35px;
    max-height: 80%;
}
.hero-right p{
 font-size: medium;
 font-weight: 100;
 color: gray;
}
.hero-left-top{
    
    background-image: url(../assets/image-web-3-desktop.jpg);
    background-size: cover;
    height: 40vh;
    
}
.hero-left-bottom{
    display: grid;
    grid-auto-flow: column;
    grid-template-columns: 0.9fr 1.1fr;
    gap: 15px;
    max-height: 25vh;
    margin-top: 15px;
    padding-top: 15px;
    
    
}

.hero-left-bottom-left h1{
    margin-top: -5px;
    font-size: 47px;
    font-weight: 900;
    
}
.hero-left-bottom-right{
    /* background-color: darkred; */
    display: flex;
    flex-direction: column;
    
    color: gray ;
    font-size: 15px;
    padding-left: 40px;
    padding-right: 20px;

}

.btn{
    background-color:hsl(5, 85%, 63%);
    color: white;
    border-style: none;
    width: 180px;
    letter-spacing: 4px;
    padding: 15px;
    margin-top: 15px;
}
.btn:hover{
    background-color:hsl(240, 100%, 5%) ;
}

</style>