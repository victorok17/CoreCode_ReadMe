**This is sixth week of CoreCode Fullstack bootcamp!**<br><br>
We started with a guided exercise using typescript and completed a couple of exercise on our own.<br><br>
Find the solution for the exercises below:<br>
*TypeScript Object Type exercise*<br>
```
export type User = {name: string, age: number, occupation: string};

export const users: User[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    }
];

export function logPerson(user: User) {
    console.log(` - ${user.name}, ${user.age}`);
}

console.log('Users:');
users.forEach(logPerson);
```

*TypeScript Unions exercise*<br>
```
```
More exercises...<br>
*Square(n) Sum exercise*<br>
```
```
*A Wolf In Sheep's Clothing exercise*<br>
```
export function warnTheSheep(queue: string[]): string {
  //1. Donde esta el lobo en el array
  //2. Correr condicionales
  //  2.1 Si el lobo esta al inicio
  //    2.1.1 "Pls go away and stop eating my sheep"
  //  2.2 Si el lobo no esta al inicio
  //    2.2.1 "Oi! Sheep number N! You are about to be eaten by a wolf!"
  //           **N es la posicion de la oveja que esta enfrente del lobo
  //======================================================================
  // 1. 
  let wolf:number = queue.indexOf('wolf');
  // 2.1
  if(++wolf === queue.length) {
    return 'Pls go away and stop eating my sheep';
  }
  // 2.2
  return `Oi! Sheep number ${queue.length - wolf}! You are about to be eaten by a wolf!`;
  
  //return ++wolf === queue.length ? 'Pls go away and stop eating my sheep' : `Oi! Sheep number ${queue.length - wolf}! You are about to be eaten by a wolf!`;
}
```
Wednesday exercises...<br>
*A Rule Of Divisibility By 13 exercise*<br>
```
```
*Playing With Digits exercise*<br>
```
```
Thursday exercises...<br>
Tile exercise
```
```
Time exercise
```
```
Rational exercise
```
```
