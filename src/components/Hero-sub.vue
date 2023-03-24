<template>
    <div class="footer">
        <div class="part-one">
            <div class="part-one-img"></div>
            <div class="part-one-text">
                <h2>01</h2>
                <h3>Reviving Retro PCs</h3>
                <p>What happens when old PCs are given modern upgrades?</p>
            </div>
        </div>
        <div class="part-two">
            <div class="part-two-img"></div>
            <div class="part-two-text">
                <h2>02</h2>
                <h3>Top 10 Laptops of 2022</h3>
                <p>Our best picks for various needs and budgets</p>
            </div>
        </div>
        <div class="part-three">
            <div class="part-three-img"></div>
            <div class="part-three-text">
                <h2>03</h2>
                <h3>The growth of Gaming</h3>
                <p>How the Pandemic has sparked fresh opportunities</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer{
    background-color: white;
    display: grid;
    grid-template-columns: 0.9fr 0.9fr 0.9fr;
    /* margin-top: 20px; */
    gap: 66px;
    color: gray;
    font-family: 'Inter', sans-serif;
    font-size: medium;
    height: 20vh;
 
}
.part-one{
 /* background-color: brown; */
 display: grid;
 grid-auto-flow: column;
 grid-template-columns: 1fr 2fr;
 
}

.part-two{
    /* background-color:aquamarine ; */
    display: grid;
    grid-auto-flow: column;
    grid-template-columns: 1fr 2fr;
}
.part-three{
    /* background-color: greenyellow; */
    display: grid;
    grid-auto-flow: column;
    grid-template-columns: 1fr 2fr;
}

.part-one-img{
    background-image: url(../assets/image-retro-pcs.jpg);
    background-size: cover;
    
    height: 130px;
    width: 80%;

}
.part-two-img{
    background-image: url(../assets/image-top-laptops.jpg);
    background-size: cover;
    
    height: 130px;
    width: 80%;
}
.part-three-img{
    background-image: url(../assets/image-gaming-growth.jpg);
    background-size: cover;
    
    height: 130px;
    width: 80%;
}
.part-one-text{
    margin-top: -23px;
}
.part-one-text p{
    font-size:smaller ;
}
.part-one-text h3{
    color: hsl(240, 100%, 5%);
}


.part-two-text{
    margin-top: -23px;
}
.part-two-text p{
    font-size:smaller ;
}
.part-two-text h3{
    color: hsl(240, 100%, 5%);
}


.part-three-text{
    margin-top: -23px;
}
.part-three-text p{
    font-size:smaller ;
}
.part-three-text h3{
    color: hsl(240, 100%, 5%);
}

@media (max-width: 800px) {
    .footer{
        display: flex;
        flex-direction: column;
        margin: 20% 3% 10% 3%;
    }
}



</style>