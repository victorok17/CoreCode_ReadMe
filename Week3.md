**This is third week of CoreCode Fullstack bootcamp!**<br><br>
Monday exercises <br>
Find below teh solutions for the exercises given:<br>
*Who Likes It?*<br>
```
function likes(names) {
  const people = ['Peter', 'Jacob', 'Alex', 'Max', 'John', 'Mark']

  if (people === 1){
     return console.log(people[0] + ' likes this')
  } 
  
  else if (people <= 2){
    return console.log(people[0] + people.length + 'like this')
  } 
  
  else if (people === 0){
     return console.log('No one like this')};
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
```
*Decode The Morse Code*<br>
```
```
Wednesday exercises <br>
Find below the solutions for the exercises given:<br>
*Simple Pig Latin*<br>
```
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
