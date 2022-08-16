**This is third week of CoreCode Fullstack bootcamp!**<br><br>
Monday exercises <br>
Find below teh solutions for the exercises given:<br>
*Who Likes It?*<br>
```
function likes(names) {
  if (names.length === 0){
    return 'no one likes this';
  }
  
  else if (names.length === 1){
     return `${names[0]} likes this`;
  } 
  
  else if (names.length === 2){
    return `${names[0]} and ${names[1]} like this`;
  } 
  
  else if (names.length === 3){
     return `${names[0]}, ${names[1]} and ${names[2]} like this`;
    }
  
  else {
  let diff = names.length - 2;
    return `${names[0]}, ${names[1]} and ${diff} others like this`
  }   
}
```
*Bit Counting*<br>
```
var countBits = function(n) {
  var n = n.toString(2).replace(/0/, "").split("")
  let count = 0;
  for (let i = 0; i < n.length; i++){
    count +=parseInt(n[i])
  }
    return count
};
```
*Your Order, Please*<br>
```
function order(words){
  if (!words) {
    return words;
  }
  var arr = words.split(' ');
  
  var obj = {}
  for (var element of arr) {
    var number = getNumber(element);
    obj[number]=element;
  }
  return Object.values(obj).join(' '); 
}

function getNumber (str){
  return str.match(/\d/)[0];
}
```
Tuesday exercises <br>
Find below the solutions for the exercises given:<br>
*Simple Pig Latin*<br>
```
function pigIt(str){
  let newArray = []
  let strArr = str.split (" ")
  strArr.forEach(x => {
    let word = x.split("");
    word.push(word[0], "ay"), word.shift()
    if (x === "!" || x === "." || x === "?"){
      newArray.push(x)    
    } else {
      newArray.push(word.join(""))
    }
  })
  return newArray.join(" ")
}
```
*Counting Duplicates*<br>
```
function duplicateCount(text){
  let count = 0
  let obj = {}
  
  for (let i of text ){
    i = i.toLowerCase()
    if (!obj[i]){
      (obj[i])=1
    } else {
      obj[i]++
    }
  }
  for (let i in obj){
    if (obj[i] > 1){
      count++
    }
  }
  return count
}

```
*Decode The Morse Code*<br>
```
decodeMorse = function(morseCode){
  return morseCode.split('  ').map(word=>{
    return word.split(' ').map(c=>MORSE_CODE[c]).join('')
  }).join(' ').trim()
}
```
Wednesday exercises <br>
Find below the solutions for the exercises given:<br>
*Valid Parantheses*<br>
```
function validParentheses(parens) {
  let openNum = 0;
  for(let i = 0; i < parens.length; i++){
    if (parens.charAt(i) == "("){
      openNum += 1;
    }else{
      openNum -= 1;
    }
    if (openNum < 0 ){
      return false;
    }   
  }
  if (openNum === 0){
    return true
  } else {
    return false;
  }
  
}
```
*Convert String To Camel Case*<br>
```
```
*Unique In Order*<br>
```
```
Thursday exercises <br>
Find below the solutions for the exercises given:<br>
*Fold An Array*<br>
```
```
*Encrypt This!*<br>
```
function encrypt(word) {
  if(word.length === 1) return `${word.charCodeAt(0)}`;
  const charBackup = word[1];
  word = word.replace(word[0], word.charCodeAt(0));
  word = word.replace(charBackup, word[word.length-1]);
  word = word.replace(/\w$/, charBackup);
  return word;
}

var encryptThis = function(text) {
  const textArray = text.split(' ');
  let result = '';
  textArray.forEach((w) => {
    // result = `${result === '' ? '' : `${result} `}${encrypt(w)}`;
    result = `${result} ${encrypt(w)}`;
  })
  return result.trim();
}
```
