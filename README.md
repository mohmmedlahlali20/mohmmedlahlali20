<style>
  /*TODO: clean it all up, finish flex, add aesthetics, icons, redefine to be relative to vh-vw, maybe rework v2 variant using scss and frames and real transitions? */
html body {
  background-color: black;
  margin: 0 0 0 0;
}
.infocardContainer * {
  font-family: 'Fira Sans Condensed', sans-serif;
  font-weight: 300;
}
h2 {
  font-weight: 600; font-style: italic; font-family: "Fira Sans Condensed", sans-serif;
}
header {
  height: 2em;
  background-color: #111122;
  margin: 0 0 0 0;
  padding: auto;
  font-size: 2em;
  text-align: center;
  line-height: 2em;
  color: white;
}
a {
  text-decoration: none;
}
a:visited {
  color: #555566;
}
a:hover {
  text-decoration: underline;
}
.infocardContainer {
  display: flex;
  height: 200px;
  width: 200px;
  border-radius: 100px;
  background: rgb(0,159,255);
  background: linear-gradient(121deg, rgba(255,255,255,0) 13%, rgba(0,159,255,1) 100%);
  transition: all 500ms ease-in;
  transition-delay: 1s;
  margin: auto;
  margin-top: 100px;
  --margin-top: 100px;
}
.infocardContainer:hover {
  width: 500px;
  border-radius: 100px 10px 100px 100px;
  transition: all 1s ease-out;
}

.infocardContainer div {
  text-color: white;
  flex-shrink: 1;
  width: 100%;
  --background-color: green;
}
.infocardContainer div * {
  display: flex;
  --flex: inherit;
  overflow: hidden;
  text-overflow: hidden;
  --background-color: yellow;
  color: white;
  white-space: nowrap;
  width: 0;
  height: auto;
  transition: all 450ms ease-in;
  transition-delay: 1s;
}
.infocardContainer:hover div *{
  --background-color: purple;
  display: flex;
  visibility: visible;
  transition: all 1s ease-out;
  transition-delay: 500ms;
  width: 100%;
  height: auto;
}

.infocardContainer #main, .infocardContainer #main img{
  --background-color: red;
  height: 200px;
  width: 200px;
  padding-right: 10px;
  border-radius: 100%;
  flex-shrink: 0;
  object-fit: cover;
}
.infocardContainer #main img{
  height: 180px;
  width: 180px;
  transition: none;
  display: float;
  position: relative;
  border: 10px solid white;
  margin: 0 0 0 0; padding: 0 0 0 0;
}
.infocardContainer #textbois {
  position: relative;
}
.infocardContainer #textbois #hotlinks {
  max-width: 60%;
  max-height: 30px;
  
  --background-color: white;
  position:absolute;
  bottom: 5px;
  display: flex;
  justify-content: space-between;
  border-radius: 13px;
}
.infocardContainer #textbois #hotlinks * {
  background-color: white;
  max-width: 30px;
  --margin: 0 1px 0 1px;
  border-radius: 25px;
}
/*TODO: animate copy main transition style for info*/
.infocardContainer #textbois #hotlinks *:hover {
  
  
}
</style>


<head>
  <link href="https://fonts.googleapis.com/css?family=Fira+Sans+Condensed:300,400,600i&display=swap" rel="stylesheet">
</head>
<header> <a href="https://codepen.io/LIMESTA/pen/VwZNmJE"> Click here to check out V2 utilizing SCSS </a> </header>
<div class="infocardContainer">
  <div id="main">
    <img src="https://upload.wikimedia.org/wikipedia/commons/e/ea/Dog_coat_variation.png"></img>
  </div>
  <div id="textbois">
    <h2>Emil Alicic</h2>
    <h4>Professional Memeologist</h4>
    <a href="mailto:limecicila@gmail.com">limecicila@gmail.com</a>
    <div id="hotlinks">
      <a href="https://codepen.io/LIMESTA"><img id="codepenio" src="https://blog.codepen.io/wp-content/uploads/2012/06/Button-Fill-Black-Small.png" target="_blank"></img>
      </a>
      <a href="https://codepen.io/LIMESTA">
        <img id="codepenio" src="https://blog.codepen.io/wp-content/uploads/2012/06/Button-Fill-Black-Small.png" target="_blank"></img>
      </a>
      <a href="https://codepen.io/LIMESTA">
        <img id="codepenio" src="https://blog.codepen.io/wp-content/uploads/2012/06/Button-Fill-Black-Small.png" target="_blank"></img>
      </a>
    </div>
  </div>
</div>
