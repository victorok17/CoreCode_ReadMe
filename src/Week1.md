
**Interpreted And Compiled Programming Languages**<br>
A Programming Language is a set of rules and instructions for a machine to execute. <br>
There are three types of Programming Languages:
1. Compiled language *is a language where the source code requires to be compiled by a program, sent to the target machine and then executed.* They are usually faster, but requires specific software to be run.
2. Interpreted language *is a language whenre the source code is directly sent to the target machine to be translated and executed by a different program.* They might be slower executed, but it is more likele to be interpreted by multiple platforms.
3. Hybrid language *combines both languages, which means that the source code is compiled, sent to the target machine and interpreted.*<br>
Java is a *Hybrid* language since it is compiled into a bytecode file (.class), sent  to the target machine where is interpreted by JVM and converts it into machine code. <br>

**Pseudocode currency converter**<br>
```
INSTRUCTIONS
Starting point: START
Input: READ, GET
Output: PRINT
Math: +, -, *, /
Assignation: <--
End point: END
```
```
Algoritmo USD_TO_BTC

Start
USD_amount <--- GET
BTC_exchange <--- 0.000043
RESULT <--- USD_amount*BTC_exchange
PRINT <--- RESULT
END
```
**My year of birth in Matrix.**<br>
I was asked to enter convert my year of birth (1996) into binary. It is 11111001100. <br>
Here's the math!![82d48588-e204-48c3-a53e-9e6a8199173c](https://user-images.githubusercontent.com/109565598/180112739-c62c819f-79cd-4048-a8a7-d93d0d95c037.jpg)

**MIPS programming language**<br>
We did a quick overview of MIPS which stands for *Microprocessor without Interlocked Pipeline Stages*. This is low-level programming language used to assembly MIPS processors.<br>
The overview included commands and instructions to create a program that displays "hello world" and a program that asks for two numbers and prints the first one.<br><br>

**Print special numbers**<br>
We were asked to create an algorithm that prints even numbers between 0 and 100. <br>
This is my resolution: <br>
```
let n = 0
for (let n = 0; n <= 100; n++){
	if (n % 2 == 0) console.log(n);
}
```
**Bad code exercise 1**<br>
The error seems to be the statament. The console prints that the variable is true, when it is false.<br>
I corrected the code and came up with the following reoslution:<br>
```
var cond = false;

if ((cond = true)) {
  console.log('The cond variable is false');
} else {
  console.log('The cond variable is true');
}
```
**Bad code exercise 2**<br>
We were asked to correct the following code: 
```
var n = 100;

if (n == 100) {
  console.log('This is a special number!');
}
if (n < 1000) {
  console.log('');
} else {
  console.log('Just a regular number');
}
if (n % 10 == 0) {
  console.log('This number is multiple of 10');
}
```
This code is supposed to print:<br>
*This a magical number* if the var value is 100<br>
*This almost a magical number* if the var value is less than 1000 and multiple of 10<br>
*This a regular number* if the var value is any other number<br><br>
So I edited it and came up with the following resolution:
```
var n = 100;

if (n == 100) 
  {console.log('This is a special number!');}
 else if (n < 1000 && n % 10 == 0)
 	{console.log('This is almost a special number!');}
else {console.log('This is a regular number!')}
```
*[Take me back to the main site](https://github.com/victorok17/CoreCode_ReadMe)*
