<template>
  <body>
    <a href="#" class="neon">Vista</a>
    <a href="#" class="neon1">Learn</a>
  </body>
</template>

<script>
</script>

<style>
:root{
  --clr--neon:hsl(201, 51%, 70%);
  --clr--bg:hsl(321, 65%, 11%);

}
*,
*::before,
*::after{
  box-sizing:inherit;
}
body{
  min-height:100vh;
  display:grid;
  place-items: center;
  background: var(--clr--bg);
  font-family:'Times New Roman', Times, serif;
  color: var(--clr--neon);
  padding-right:10rem;
}
.neon{
   font-size: 3rem;
   display:inline-block;
   cursor:pointer;
   text-decoration: none;
   color:var(--clr--neon);
   border:currentColor 0.125em solid;
   padding: 0.25em 1.25em;
   border-radius: 0.25em;
  
   text-shadow: 
   0 0 0.125em hsl(0 0% 100% / 0.5),
   0 0 0.45em currentColor; 
   
   box-shadow: 
   0 0 0.125em hsl(0 0% 100% / 0.5),
   0 0 0.45em currentColor; 
   position: relative;
   transition: background-color 0.3s
   linear;
}
.neon::before{
pointer-events: none;
  content:""; 
  position: absolute;
  background: var(--clr--neon);
    top:120%;
    left:0;
    width:100%;
    height: 100%;

 
transform:perspective(1em) rotateX(40deg) scale(1, 0.35);
filter: blur(1em);
opacity: 0.7;
}

.neon::after{
content: '';
position:absolute;
top:0;
bottom:0;
left:0;
right:0;
box-shadow: 0 0 2em 0.5 var(--clr--neon);
opacity: 0;
transition: opacity 100ms linear;
}


.neon:hover{
  background: var(--clr--neon);
  color: var(--clr--bg); 
  text-shadow: none;
}
.neon:hover::after
{
  opacity: 1;
}
.neon1{
   font-size: 3rem;
   display:inline-block;
   margin-left:44pc;
   margin-top:-39pc;
   cursor:pointer;
   text-decoration: none;
   color:var(--clr--neon);
   border:currentColor 0.125em solid;
   padding: 0.25em 1.25em;
   border-radius: 0.25em;
  
   text-shadow: 
   0 0 0.125em hsl(0 0% 100% / 0.5),
   0 0 0.45em currentColor; 
   
   box-shadow: 
   0 0 0.125em hsl(0 0% 100% / 0.5),
   0 0 0.45em currentColor; 
   position: relative;
   transition: background-color 0.3s 
   linear;
}
.neon1::before{
pointer-events: none;
  content:""; 
  position: absolute;
  background: var(--clr--neon);
    top:120%;
    left:0;
    width:100%;
    height: 100%;

 
transform:perspective(1em) rotateX(40deg) scale(1, 0.35);
filter: blur(1em);
opacity: 0.7;
}
.neon1::after{
content: '';
position:absolute;
top:0;
bottom:0;
left:0;
right:0;
box-shadow: 0 0 2em 0.5 var(--clr--neon);
opacity: 0;
transition: opacity 100ms linear;
}
.neon1:hover{
  background: var(--clr--neon);
  color: var(--clr--bg); 
  text-shadow: none;
}
.neon1:hover::after
{
  opacity: 1;
}
</style>
