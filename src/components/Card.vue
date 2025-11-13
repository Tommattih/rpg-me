<template>
    <div class="deck">
        <div class="card-back blue"></div>
        <div class="card-back horizontal-top"></div>
        <div class="card-back green"></div>
        <div class="card-back vertical-right"></div>
        <div class="card-front">
            <h2>Card Title</h2>
            <img src="" alt="ilustration">
            <p>This is a sample card component.</p>
            <div class="stacks">num</div>
        </div>
        <div class="card-back vertical-left"></div>        
        <div class="card-back pink"></div>
        <div class="card-back horizontal-bottom"></div>
        <div class="card-back orange"></div>
    </div>
</template>

<style scoped>
.card-back, .card-front{
    width: 10rem;
    height: 18rem;
    border : 1px double darkslategrey;
    border-radius: .5rem;
}
.card-back{
    background-color: #222;
}
.deck {
    display: flex;
    gap: 1rem;
    margin-bottom: 1rem;
    flex-wrap: wrap;
    justify-content: center;
}

.blue {
    background: 
      linear-gradient(145deg,#2847d3 10%,#4b8aa6 10.5% 19%,#0000 19.5% 80.5%,#4b8aa6 81% 89.5%,#352389 90%), 
      linear-gradient(145deg,#2847d3 10%,#4b8aa6 10.5% 19%,#0000 19.5% 80.5%,#4b8aa6 81% 89.5%,#352389 90%) calc(28px) 56px,
      linear-gradient(35deg,#2847d3 10%,#4b8aa6 10.5% 19%,#0000 19.5% 80.5%,#4b8aa6 81% 89.5%,#352389 90%), 
      linear-gradient( 35deg,#2847d3 10%,#4b8aa6 10.5% 19%,#0000 19.5% 80.5%,#4b8aa6 81% 89.5%,#352389 90%) calc(28px) 56px,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#2847d3 0) calc(28px/4) 0,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#352389 0) calc(28px) 0,
      linear-gradient(90deg,#352389 38%,#2847d3 0 50%,#352389 0 62%,#2847d3 0);
      
    background-size: 56px calc(2*56px/3);
}

.pink {
    background: 
      linear-gradient(145deg,#782f67 10%,#c75b5b 10.5% 19%,#0000 19.5% 80.5%,#c75b5b 81% 89.5%,#352389 90%), 
      linear-gradient(145deg,#782f67 10%,#c75b5b 10.5% 19%,#0000 19.5% 80.5%,#c75b5b 81% 89.5%,#352389 90%) calc(28px) 56px,
      linear-gradient(35deg,#782f67 10%,#c75b5b 10.5% 19%,#0000 19.5% 80.5%,#c75b5b 81% 89.5%,#352389 90%), 
      linear-gradient( 35deg,#782f67 10%,#c75b5b 10.5% 19%,#0000 19.5% 80.5%,#c75b5b 81% 89.5%,#352389 90%) calc(28px) 56px,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#782f67 0) calc(28px/4) 0,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#352389 0) calc(28px) 0,
      linear-gradient(90deg,#352389 38%,#782f67 0 50%,#352389 0 62%,#782f67 0);
      
    background-size: 56px calc(2*56px/3);
}
.orange {
    background: 
      linear-gradient(145deg,#c75b5b 10%,#ff9c13 10.5% 19%,#0000 19.5% 80.5%,#ff9c13 81% 89.5%,#a53013 90%), 
      linear-gradient(145deg,#c75b5b 10%,#ff9c13 10.5% 19%,#0000 19.5% 80.5%,#ff9c13 81% 89.5%,#a53013 90%) calc(28px) 56px,
      linear-gradient(35deg,#c75b5b 10%,#ff9c13 10.5% 19%,#0000 19.5% 80.5%,#ff9c13 81% 89.5%,#a53013 90%), 
      linear-gradient( 35deg,#c75b5b 10%,#ff9c13 10.5% 19%,#0000 19.5% 80.5%,#ff9c13 81% 89.5%,#a53013 90%) calc(28px) 56px,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#c75b5b 0) calc(28px/4) 0,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#a53013 0) calc(28px) 0,
      linear-gradient(90deg,#a53013 38%,#c75b5b 0 50%,#a53013 0 62%,#c75b5b 0);
    background-size: 56px calc(2*56px/3);

}

.green {
    background: 
      linear-gradient(145deg,#ff9c13 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#4b8aa6 90%), 
      linear-gradient(145deg,#ff9c13 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#4b8aa6 90%) calc(28px) 56px,
      linear-gradient(35deg,#ff9c13 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#4b8aa6 90%), 
      linear-gradient( 35deg,#ff9c13 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#4b8aa6 90%) calc(28px) 56px,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#ff9c13 0) calc(28px/4) 0,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#4b8aa6 0) calc(28px) 0,
      linear-gradient(90deg,#4b8aa6 38%,#ff9c13 0 50%,#4b8aa6 0 62%,#ff9c13 0);
    background-size: 56px calc(2*56px/3);
}
.horizontal-top {
    background: 
      linear-gradient(145deg,#2847d3 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#4b8aa6 90%), 
      linear-gradient(145deg,#2847d3 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#4b8aa6 90%) calc(28px) 56px,
      linear-gradient(35deg,#2847d3 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#4b8aa6 90%), 
      linear-gradient( 35deg,#2847d3 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#4b8aa6 90%) calc(28px) 56px,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#2847d3 0) calc(28px/4) 0,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#4b8aa6 0) calc(28px) 0,
      linear-gradient(90deg,#4b8aa6 38%,#2847d3 0 50%,#4b8aa6 0 62%,#2847d3 0);
    background-size: 56px calc(2*56px/3);
}
.horizontal-bottom {
    background: 
      linear-gradient(145deg,#c75b5b 10%,#a53013 10.5% 19%,#0000 19.5% 80.5%,#a53013 81% 89.5%,#782f67 90%), 
      linear-gradient(145deg,#c75b5b 10%,#a53013 10.5% 19%,#0000 19.5% 80.5%,#a53013 81% 89.5%,#782f67 90%) calc(28px) 56px,
      linear-gradient(35deg,#c75b5b 10%,#a53013 10.5% 19%,#0000 19.5% 80.5%,#a53013 81% 89.5%,#782f67 90%), 
      linear-gradient( 35deg,#c75b5b 10%,#a53013 10.5% 19%,#0000 19.5% 80.5%,#a53013 81% 89.5%,#782f67 90%) calc(28px) 56px,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#c75b5b 0) calc(28px/4) 0,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#782f67 0) calc(28px) 0,
      linear-gradient(90deg,#782f67 38%,#c75b5b 0 50%,#782f67 0 62%,#c75b5b 0);
    background-size: 56px calc(2*56px/3);
}
.vertical-left {
    background: 
      linear-gradient(145deg,#ff9c13 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#a53013 90%), 
      linear-gradient(145deg,#ff9c13 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#a53013 90%) calc(28px) 56px,
      linear-gradient(35deg,#ff9c13 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#a53013 90%), 
      linear-gradient( 35deg,#ff9c13 10%,#dec1b5 10.5% 19%,#0000 19.5% 80.5%,#dec1b5 81% 89.5%,#a53013 90%) calc(28px) 56px,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#ff9c13 0) calc(28px/4) 0,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#a53013 0) calc(28px) 0,
      linear-gradient(90deg,#a53013 38%,#ff9c13 0 50%,#a53013 0 62%,#ff9c13 0);
    background-size: 56px calc(2*56px/3);

}
.vertical-right {
    background: 
      linear-gradient(145deg,#352389 10%,#2847d3 10.5% 19%,#0000 19.5% 80.5%,#2847d3 81% 89.5%,#782f67 90%), 
      linear-gradient(145deg,#352389 10%,#2847d3 10.5% 19%,#0000 19.5% 80.5%,#2847d3 81% 89.5%,#782f67 90%) calc(28px) 56px,
      linear-gradient(35deg,#352389 10%,#2847d3 10.5% 19%,#0000 19.5% 80.5%,#2847d3 81% 89.5%,#782f67 90%), 
      linear-gradient( 35deg,#352389 10%,#2847d3 10.5% 19%,#0000 19.5% 80.5%,#2847d3 81% 89.5%,#782f67 90%) calc(28px) 56px,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#352389 0) calc(28px/4) 0,
      conic-gradient(from -90deg at 37.5% 50%,#0000 75%,#782f67 0) calc(28px) 0,
      linear-gradient(90deg,#782f67 38%,#352389 0 50%,#782f67 0 62%,#352389 0);
    background-size: 56px calc(2*56px/3);

}

</style>