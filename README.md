<!DOCTYPE html>
<html lang="en">
    
<script>
    window.addEventListener( 'DOMContentLoaded', function () {

const buttonRoolDice = document.querySelector( '.dice-roll' );

function rollDice () {

const diceSide1 = document.getElementById( 'dice-side-1' );
const diceSide2 = document.getElementById( 'dice-side-2' );
const status = document.getElementById( 'status' );

const side1 = Math.floor( Math.random() * 6 ) + 1;
const side2 = Math.floor( Math.random() * 6 ) + 1;
const diceTotal = side1 + side2;

diceSide1.innerHTML = side1;
diceSide2.innerHTML = side2;

status.innerHTML = 'You rolled ' + diceTotal + '.';

if ( side1 === side2 ) {
status.innerHTML += ' Doubles! You get a free turn!';
}
}

buttonRoolDice.addEventListener( 'click', rollDice, false );

}, false);

    
    </script>
    
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="aboutme.css" rel="stylesheet">
    <title>Document</title>
</head>
 
<body>
    <div id="wrapper">
        <header>
   <h1>Jamal Coates</h1>
             </header>
   
   
    
    <main>
   
    <p>
        <b>About Me:</b>
        <br>I am an artist by nature. i believe everyone is. I believe everyone has the urge to create or at least recreate and express themselves whether it be painting, music, decorating and designing.<br> 
        Since I was 3 years old i have been drawing or doodling to the point where it got me detention for not doing work but drawing instead. I began to focus on sports and music as I grew and put art on the back burner until I was approached by an old classmate who wanted a logo designed for her company. I didn't know how to use Adobe Illustrator but I got the job done and it was a success. Now I am a full time student to learn graphic design so i can show the world my creations. 
        </p>
        
        <p><b>My favorite quote is:</b>
         <em>"If you feed it, it will grow."</em>
         
        
</main>  
    <div class="wrapper">
<div class="column">
<div id="dice-side-1" class="dice">0</div>
<div id="dice-side-2" class="dice">0</div>
</div>
<div class="column">
<button type="button" class="dice-roll">roll dice</button>
<h2 id="status"></h2>
</div>
</div>    
<em>Copyright &copy; Jamal Coates 2018</em>
</div> 
</body>

</html>
