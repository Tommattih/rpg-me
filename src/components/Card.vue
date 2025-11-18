<template>
  <div class="deck">
    <div class="card-back blue"></div>
    <div class="card-back horizontal-top"></div>
    <div class="card-back green"></div>
    <div class="card-back vertical-right"></div>
    <div class="card-front">
      <div class="card-frame"></div>
      <div class="card-img-container">
        <img src="https://plus.unsplash.com/premium_photo-1683910767532-3a25b821f7ae?w=800&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MXx8aW1hZ2VucyUyMGdyYXR1aXRhc3xlbnwwfHwwfHx8MA%3D%3D" alt="ilustration">
      </div>

            <div class="card-name">
        <h2>Card Title</h2>
      </div>
      
      <div class="card-description">
        <p>This is a sample card component.</p>
      </div>

      <div class="card-values">
        <div class="card-number">
          <span>000</span>
        </div>
        
        <div class="card-stacks">
          <ul>
            <li>aa</li>
            <li>bb</li>
          </ul>
        </div>
      </div>
    </div>
      
            
    <div class="card-back vertical-left"></div>        
    <div class="card-back pink"></div>
    <div class="card-back horizontal-bottom"></div>
    <div class="card-back orange"></div>
  </div>
</template>

<style scoped>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
.deck {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
  justify-content: center;
  padding: 2rem;
  background-color: #1a1a1a;
}
.card-back, .card-front{
    width: 12rem;
    height: 18rem;
    border : 2px double rgb(43, 47, 66);
    border-radius: .25rem;
    position: relative;
    overflow: hidden;
    box-shadow: 2px 4px 6px rgb(0, 0, 0, 0.5);
}
.card-back{
    background-color: #222;
}

/* BACK STYLES */
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
/* FRONT DETAILS */
.card-front {
  display: grid;
  grid-template-rows: 1fr auto;
  color: white; /* rever */
}
.card-front::before {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(145deg, #2847d3 10%, #dec1b5 10.5% 19%, #0000 19.5% 80.5%, #dec1b5 81% 89.5%, #4b8aa6 90%), linear-gradient(145deg, #2847d3 10%, #dec1b5 10.5% 19%, #0000 19.5% 80.5%, #dec1b5 81% 89.5%, #4b8aa6 90%) calc(28px) 56px, linear-gradient(35deg, #2847d3 10%, #dec1b5 10.5% 19%, #0000 19.5% 80.5%, #dec1b5 81% 89.5%, #4b8aa6 90%), linear-gradient(35deg, #2847d3 10%, #dec1b5 10.5% 19%, #0000 19.5% 80.5%, #dec1b5 81% 89.5%, #4b8aa6 90%) calc(28px) 56px, conic-gradient(from -90deg at 37.5% 50%, #0000 75%, #2847d3 0) calc(28px / 4) 0, conic-gradient(from -90deg at 37.5% 50%, #0000 75%, #4b8aa6 0) calc(28px) 0, linear-gradient(90deg, #4b8aa6 38%, #2847d3 0 50%, #4b8aa6 0 62%, #2847d3 0);
  background-size: 56px calc(2 * 56px / 3);
  filter: blur(3px);
  z-index: 0;
  pointer-events: none;
}
.card-img-container {
 position: absolute;
 top: 0.25rem;
 left: 0;
 z-index: 5;
 width: 100%;
 height: 72.5%;
 clip-path: polygon(5% 3%, 20% 5%, 25% 15%, 75% 15%, 80% 5%, 95% 3%, 94% 75%, 83% 75%, 75% 85%, 30% 85%, 21% 75%, 6% 75%);
}

.card-img-container img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.card-name {
  position: relative;
  z-index: 3;
  text-align: center;
  margin-top: .15rem;
}
/* NAME BACKGROUND */
.card-name::before {
  content: '';
  position: absolute;
  background: #4b8aa6;
  opacity: 0.8;
  top: .5rem;
  bottom: 1rem;
  right: 2.2rem;
  left: 2.2rem;
  z-index: -1;
  clip-path: polygon(0 0, 100% 0, 90% 15%, 10% 15%);
  border-top: solid 4px #2847d3;
}
.card-name h2 {
  display: inline-block;
  margin-top: .85rem;
  font-size: 0.7rem;
  text-transform: uppercase; /* Capitalize talvez */
}

.card-description {
  position: relative;
  z-index: 2;
  text-align: start;
  font-size: .6rem;
  height: 5.9rem;
  width: 100%;
  right: 0.25rem;
  color: #222;
  font-weight: 600;
  padding: 0 3rem 1.25rem 1.25rem;
}
/* DESCRIPTION BACKGROUND */
.card-description::before {
  content: '';
  position: absolute;
  z-index: -1;
  left: .75rem;
  right: 0.7rem;
  top: -.58rem;
  bottom: 0.5rem;
  opacity: 0.75;
  background: #dec1b5; /*var*/
}
  
  .card-values {
  position: absolute;
  inset: 0;
  z-index: 4;
  pointer-events: none;
}
.card-number {
  position: absolute;
  left: 0.5rem;
  right: 7.6rem;
  bottom: 6.25rem;
  height: 1.65rem;
  display: flex;
  justify-content: start;
  align-items: center;
  font-size: .75rem;
  font-weight: 800;
  clip-path: polygon(0 0, 50% 0, 90% 90%, 0% 90%);
  border-top: double 4px #4b8aa6;
  border-left: solid 4px #dec1b5;
}
/* NUMBER BACKGROUND */
.card-number::before {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  background-color: #4b8aa6;
  opacity: 0.8;
  z-index: -1;
  /* border-left: solid 4px #2847d3;var */
}
.card-number span {
  padding: .5rem .5rem;
}

.card-stacks {
  position: absolute;
  right: .5rem;
  bottom: .5rem;
  left: 4.75rem;
  top: 9.85rem;
  clip-path: polygon(79% 0, 100% 0, 100% 100%, 75% 100%, 60% 20%);
}
.card-stacks::before {
  content: '';
  position: absolute;
  right: -.05rem;
  left: 2rem;
  height: 95%;
  opacity: 0.9;
  z-index: -1;
  background-color: #4b8aa6;
  border: solid 4px #2847d3;
  border-bottom: solid 2px #dec1b5;
  border-top: double 4px #dec1b5;/* var*/
}
  .card-stacks ul {
  list-style: none;
  text-align: end;
  font-size: .8rem;
  font-weight: 600;
  padding: .5rem .5rem;
}
.card-frame{
  content: '';
  position: absolute;
  inset: .25rem 4px .2rem;
  border: dashed 1px #dec1b4;
}
</style>