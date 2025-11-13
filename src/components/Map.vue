<template>
        <nav id="worlds">
            <div class="lands">
                <div class="div1"> 1</div>
                <div class="div2"> 2</div>
                <div class="div3"> 3</div>
                <div class="div4"> 4</div>
                <div class="div5"> 5</div>
                <div class="div6"> 6</div>
                <div class="div7"> 7</div>
                <div class="div8"> 8</div>
                <div class="div9"> <a id="portal" href="#rpg_me">
                    <div class="cssload-loader">
                        <div class="cssload-inner cssload-one"></div>
                        <div class="cssload-inner cssload-two"></div>
                        <div class="cssload-inner cssload-three"></div>
                    </div>
                </a></div>
            </div>
        </nav>
</template>

<style scoped>



/* designed with https://cssgrid-generator.netlify.app/ */
.lands {
    display: grid;
    grid-template-columns: 3fr 2fr 3fr;
    grid-template-rows: 3fr 2fr 3fr;
    grid-column-gap: 0;
    grid-row-gap: 0;
    justify-items: center;
    align-items: center;
}

.div1 { grid-area: 1 / 1 / 2 / 2; }
.div2 { grid-area: 1 / 3 / 2 / 4; }
.div3 { grid-area: 3 / 3 / 4 / 4; }
.div4 { grid-area: 3 / 1 / 4 / 2; }
.div5 { grid-area: 2 / 1 / 3 / 2; }
.div6 { grid-area: 1 / 2 / 2 / 3; }
.div7 { grid-area: 2 / 3 / 3 / 4; }
.div8 { grid-area: 3 / 2 / 4 / 3; }
.div9 { grid-area: 2 / 2 / 3 / 3; }
/* designed with https://cssgrid-generator.netlify.app/ */


/* 1) Contêiner principal */
#worlds {
  background-color: #05051d;
  width: 100%;
  margin: 2rem auto;
  padding: .5rem;
  overflow: hidden;
  box-sizing: border-box;
}

/* 2) Grade de mapa 3x3 */
.lands {
  display: grid;
  grid-template-columns:
    minmax(6rem, 3fr)
    minmax(4rem, 2fr)
    minmax(6rem, 3fr);
  grid-template-rows:
    minmax(6rem, 3fr)
    minmax(4rem, 2fr)
    minmax(6rem, 3fr);

  /* espaçamento entre as divs */
  gap: 0.25rem;
  
  margin: 0 auto;
  width: 80%;
  aspect-ratio: 1 / 1;   /* mantém a forma quadrada */
  justify-items: center;
  align-items: center;
}

/* 3) Células individuais */
.lands > div {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: .25rem;
  
  color: #fff;
  background-color: #111;
  border: 1px solid #333;
  border-radius: 5%;
  box-sizing: border-box;

  /* sombra leve pra separar visualmente */
  box-shadow: 0 0 .25rem rgba(255,255,255,0.05);
}

/* MERAMENTE ILUSTRATIVO */
.lands .div6 {background-color: #4b8aa6;}
.lands .div8 {background-color: #c75b5b;}
.lands .div4 {background-color: #a53013;}
.lands .div5 {background-color: #ff9c13;}
.lands .div1 {background-color: #dec1b5;}
.lands .div3 {background-color: #782f67;}
.lands .div7 {background-color: #352389;}
.lands .div2 {background-color: #2847d3;}
/* MERAMENTE ILUSTRATIVO */

.lands .div9 {
  border: none;
  background: none;
}

.cssload-loader {
	position: relative;
	left: calc(50% - 31px);
	width: 4rem;
	height: 4rem;
	border-radius: 50%;
		-o-border-radius: 50%;
		-ms-border-radius: 50%;
		-webkit-border-radius: 50%;
		-moz-border-radius: 50%;
	perspective: 780px;
}

.cssload-inner {
	position: absolute;
	width: 100%;
	height: 100%;
	box-sizing: border-box;
		-o-box-sizing: border-box;
		-ms-box-sizing: border-box;
		-webkit-box-sizing: border-box;
		-moz-box-sizing: border-box;
	border-radius: 50%;
		-o-border-radius: 50%;
		-ms-border-radius: 50%;
		-webkit-border-radius: 50%;
		-moz-border-radius: 50%;	
}

.cssload-inner.cssload-one {
	left: 0%;
	top: 0%;
	animation: cssload-rotate-one 1.15s linear infinite;
		-o-animation: cssload-rotate-one 1.15s linear infinite;
		-ms-animation: cssload-rotate-one 1.15s linear infinite;
		-webkit-animation: cssload-rotate-one 1.15s linear infinite;
		-moz-animation: cssload-rotate-one 1.15s linear infinite;
	border-bottom: 3px solid rgba(199,226,255,0.98);
}

.cssload-inner.cssload-two {
	right: 0%;
	top: 0%;
	animation: cssload-rotate-two 1.15s linear infinite;
		-o-animation: cssload-rotate-two 1.15s linear infinite;
		-ms-animation: cssload-rotate-two 1.15s linear infinite;
		-webkit-animation: cssload-rotate-two 1.15s linear infinite;
		-moz-animation: cssload-rotate-two 1.15s linear infinite;
	border-right: 3px solid rgb(255, 254, 197);
}

.cssload-inner.cssload-three {
	right: 0%;
	bottom: 0%;
	animation: cssload-rotate-three 1.15s linear infinite;
		-o-animation: cssload-rotate-three 1.15s linear infinite;
		-ms-animation: cssload-rotate-three 1.15s linear infinite;
		-webkit-animation: cssload-rotate-three 1.15s linear infinite;
		-moz-animation: cssload-rotate-three 1.15s linear infinite;
	border-top: 3px solid rgb(103, 212, 255);
}

@keyframes cssload-rotate-one {
	0% {
		transform: rotateX(35deg) rotateY(-45deg) rotateZ(0deg);
	}
	100% {
		transform: rotateX(35deg) rotateY(-45deg) rotateZ(360deg);
	}
}

@-o-keyframes cssload-rotate-one {
	0% {
		-o-transform: rotateX(35deg) rotateY(-45deg) rotateZ(0deg);
	}
	100% {
		-o-transform: rotateX(35deg) rotateY(-45deg) rotateZ(360deg);
	}
}

@-ms-keyframes cssload-rotate-one {
	0% {
		-ms-transform: rotateX(35deg) rotateY(-45deg) rotateZ(0deg);
	}
	100% {
		-ms-transform: rotateX(35deg) rotateY(-45deg) rotateZ(360deg);
	}
}

@-webkit-keyframes cssload-rotate-one {
	0% {
		-webkit-transform: rotateX(35deg) rotateY(-45deg) rotateZ(0deg);
	}
	100% {
		-webkit-transform: rotateX(35deg) rotateY(-45deg) rotateZ(360deg);
	}
}

@-moz-keyframes cssload-rotate-one {
	0% {
		-moz-transform: rotateX(35deg) rotateY(-45deg) rotateZ(0deg);
	}
	100% {
		-moz-transform: rotateX(35deg) rotateY(-45deg) rotateZ(360deg);
	}
}

@keyframes cssload-rotate-two {
	0% {
		transform: rotateX(50deg) rotateY(10deg) rotateZ(0deg);
	}
	100% {
		transform: rotateX(50deg) rotateY(10deg) rotateZ(360deg);
	}
}

@-o-keyframes cssload-rotate-two {
	0% {
		-o-transform: rotateX(50deg) rotateY(10deg) rotateZ(0deg);
	}
	100% {
		-o-transform: rotateX(50deg) rotateY(10deg) rotateZ(360deg);
	}
}

@-ms-keyframes cssload-rotate-two {
	0% {
		-ms-transform: rotateX(50deg) rotateY(10deg) rotateZ(0deg);
	}
	100% {
		-ms-transform: rotateX(50deg) rotateY(10deg) rotateZ(360deg);
	}
}

@-webkit-keyframes cssload-rotate-two {
	0% {
		-webkit-transform: rotateX(50deg) rotateY(10deg) rotateZ(0deg);
	}
	100% {
		-webkit-transform: rotateX(50deg) rotateY(10deg) rotateZ(360deg);
	}
}

@-moz-keyframes cssload-rotate-two {
	0% {
		-moz-transform: rotateX(50deg) rotateY(10deg) rotateZ(0deg);
	}
	100% {
		-moz-transform: rotateX(50deg) rotateY(10deg) rotateZ(360deg);
	}
}

@keyframes cssload-rotate-three {
	0% {
		transform: rotateX(35deg) rotateY(55deg) rotateZ(0deg);
	}
	100% {
		transform: rotateX(35deg) rotateY(55deg) rotateZ(360deg);
	}
}

@-o-keyframes cssload-rotate-three {
	0% {
		-o-transform: rotateX(35deg) rotateY(55deg) rotateZ(0deg);
	}
	100% {
		-o-transform: rotateX(35deg) rotateY(55deg) rotateZ(360deg);
	}
}

@-ms-keyframes cssload-rotate-three {
	0% {
		-ms-transform: rotateX(35deg) rotateY(55deg) rotateZ(0deg);
	}
	100% {
		-ms-transform: rotateX(35deg) rotateY(55deg) rotateZ(360deg);
	}
}

@-webkit-keyframes cssload-rotate-three {
	0% {
		-webkit-transform: rotateX(35deg) rotateY(55deg) rotateZ(0deg);
	}
	100% {
		-webkit-transform: rotateX(35deg) rotateY(55deg) rotateZ(360deg);
	}
}

@-moz-keyframes cssload-rotate-three {
	0% {
		-moz-transform: rotateX(35deg) rotateY(55deg) rotateZ(0deg);
	}
	100% {
		-moz-transform: rotateX(35deg) rotateY(55deg) rotateZ(360deg);
	}
}

</style>