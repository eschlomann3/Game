<head> 
<body>
  
<h1>Guess The Number</h1> 
  
<p> Can you guess the number between 1-100? Play to see how many guesses you get!</p> 
  
<div class="form"> 
    <label for="guessField">Enter a guess: </label> 
    <input type = "text" id = "guessField" class = "guessField"> 
    <input type = "submit" value = "Try" 
           class = "guessSubmit" id = "submitguess"> 
</div> 
  
<script type = "text/javascript"> 
    var y = Math.floor(Math.random() * 100 + 1); 
    var guess = 1; 
      
    document.getElementById("submitguess").onclick = function(){      
    var x = document.getElementById("guessField").value; 
  
   if(x == y) 
   {    
       alert("CONGRATULATIONS!!! You guessed it in "
               + guess + " guesses! "); 
   } 
   else if(x > y) 
   {     
       guess++; 
       alert("Try a lower number!"); 
   } 
   else
   { 
       guess++; 
       alert("Try a higher number!") 
   } 
} 
</script>
</body> 
 
