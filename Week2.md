**This is second week of CoreCode Fullstack bootcamp!**<br>
The first activity was to do research about Js conditions, loops and functions. So, by reading MDN, I learnt that there are three types of conditions:
- If: *executes a statement if a condition is thruthy.*
- If... else *executes a statement whether the condition is truthy or falsy.*
- Else if *specifies more conditions*<br>

A function is a group of instructions that complete a task or calculate a value.<br>

Loops are cicles that repeated until a condition is truthy. There are three types of loops:<br>
- For *is a loop that consists in three expressions and finishes when they are all three completed.*<br>
- While *executes a specific instruction as long as the condition is truthy.*<br>
- Do...while *executes the code until the condition is truthy at least one time.*<br>

**Exercises**<br>
*Solution to multiply exercise:*<br>
```
function multiply(a, b){
  return a * b
}
console.log(multiply (2, 2));
```
*Solution to ASCII total exercise:*<br>
```
function uniTotal (word) {
  let long = word.length;
  let total = 0;
  for (let i = 0; i < long; i++){
    total = total + word.charCodeAt(i);
  }
  return total;
}
```
**More exercises...**<br>
*Solution to Char From ASCII Value:*<br>
```
function getChar(num){
  return String.fromCharCode(num)
}

console.log (getChar (65));
```
*Solution to Binary Addition exercise:*<br>
```
```
*Solution to Student's Final Grade exercise:*<br>
```
function finalGrade (a, b) {
  if (a > 90 || b > 10) {
    result='100';
  }
  
  else if (a > 75 && b >= 5)
    {
    result='90';
  }
  
  else if (a > 50 && b >= 2)
    {
    result='75';
  }
  
  else {
    result='0';
  }
  return result;
}
console.log(finalGrade(1,0)); 
```
**More exercises...**<br>
*Remove All Exclamation Marks From The End Of Sentence:*<br>
```
```
*Vowel Remover:*<br>
```
```
*Rock Paper Scissors!*<br>
```
const rps = (p1, p2) => {
  if (p1 === 'rock' && p2 === 'scissors') return 'Player 1 won!';
  if  (p1 === 'scissors' && p2 === 'paper') return  'Player 1 won!';
  if  (p1 === 'paper' && p2 === 'rock') return  'Player 1 won!';
  if  (p1 === p2) return "Draw!";
  return ('Player 2 won!');
};
```
*Persistent Bugger:*<br>
```
```



