# colorflip
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>colorflip</title>
    <link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Hanalei&family=Lexend+Mega&display=swap" rel="stylesheet">
</head>
<script src="simple.js">

</script>
<style>
  body{
    background-color: #f875aa;
    
  }
  .head{
    color: #000000;
    font-family: 'Hanalei', cursive;
font-family: 'Lexend Mega', sans-serif; 

 }
nav{
  background-color: #fbaccc;
  height: 40px;
  width: 100px;
  padding-left:0%;
  margin: 0%;
  padding-left: 9px;
  border-radius: 12px;
  display: inline-table;
  flex-direction: ro


}
.in{
  color: #000000;
  font-size: 24px;
  text-decoration: none;
  align-content: center;
  display: inline-block;
  padding-top: 8px;
  padding-left: 9px;
  
  font-style: oblique;
}
nav:hover {
  background-color: #be498a;
  background-size: inherit;
  color: bisque;
  transition:all 300ms ease-in-out;
}
.he{
  color: #000000;
  font-size: 24px;
  text-decoration: none;
  align-content: center;
  display: inline-block;
  padding-top: 8px;
  padding-left: 19px;
  
  font-style: oblique;
}
.container{
  display: flex;
  justify-content: center;
  align-content: center;
  padding-top: 140px;
  flex-direction: column;
  padding-left: 850px;

}
.back{
 
  height: 50px;
  width: 190px;
  padding: 10px;
  padding: 20px;
  color: rgb(0, 0, 0);
  font-weight: bold;;
  background-color: #fbaccc;

  font-style: inherit;
  font-size: 23px;  border-radius: 12px;

}
#btn
{
  width: fit-content;
  margin: 12px;
  margin-left: 70px;
  color: rgb(255, 251, 251);
  background-color: #382b2b;
  border: solid rgb(44, 33, 33);
  border-radius: 12px;
}

</style>
<script>
const colors=["red","green","blue","orange","violet"];
const bton=document.querySelectorAll('#btn');
const colour=document.getElementById("color");
console.log(bton);
bton.addEventListener("click",function(){
    const randomnum=getrandomnum();
    console.log("kalki")
    document.body.style.backgroundColor=colors[randomnum];
    colour.textContent=colors[randomnum];
})
function getrandnum()
{
    return Math.floor(Math.random()*colors.length);
}
</script>

<body >
  <h2 class="head">ColorFlipper</h2>

  <nav class="na" >
    <a class="in" href="index.html">Simple</a>
  </nav>  
  <nav>   
       <a class="he" href="hex.html">Hex</a>
  </nav>
  <div class="container">
    <div class="back" color=#000000>
      Background-color: <div id="color">#kmiewf</div>
    </div>
    <button id="btn" >Click me</button>
  </div>
</body>
</html> 
