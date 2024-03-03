### Виведіть у консоль усі числа у проміжку від 1 до 1000, сума першої та другої цифри яких дорівнює п'яти

```sh
for(let i = 1; i <= 1000; i++){
    if(i > 13 && i < 510){
        const n = i.toString()
        if(+n[0] + +n[1] === 5){
            console.log(i)

        }
    }
}
```
### Даний масив. Видаліть із нього елементи із заданим значенням.
```sh

 const arr = [1, 2, 3, 4, 5, 5, 1, 2, 3, 4, 5, 6]


console.log(arr)
function delateElement (array, e){
    while(array.indexOf(e) > 0){
        arr.splice(array.indexOf(e), 1)
    }
}

function delateElement (array, e){
        arr.splice(array.indexOf(e), 1)
        if(arr.indexOf(e) > 0) 
            return delateElement(array, e)
}

delateElement(arr, 5)
delateElement(arr, 2)
delateElement(arr, 4)
delateElement(arr, 1)
delateElement(arr, 3)
```

### Дан массив с числами. Оставьте в нем только положительные числа.
```sh
 const arr = [1, 2, -3, 4, 5, 5, -1, 2, -3, -4, 5, 6];
 const arr2 = [];

 for(let i = 0; i < arr.length; i++){
    if(arr[i] > 0){
        arr2.push(arr[i])
    }
 }
 console.log(arr2)

while(arr.findIndex((e)=> e < 0)>=0){
    arr.splice(arr.findIndex((e)=> e < 0), 1)
}


console.log(arr)
```
### Дано рядок. Видаліть передостанній символ із цього рядка
```sh
const str  = "hello world"
const str2 = str.slice(0, -2) + str.slice(-1)
console.log(str2)
```
### Даний деякий масив, наприклад, ось такий:
[1, 2, 3, 4, 5, 6]
#### Поділіть суму першої половини елементів цього масиву на суму другої половини елементів.
```sh
const arr = [2, 8, 9, 6, 3, 4, 7, 8];
let sum1 = 0;
let sum2 = 0;

arr.forEach((e, i, arr)=>{
    if(arr.length /2 > i)
        sum1 += e;
    else
        sum2 += e;
})
```
### Дано числа, розділені комами. Знайдіть суму цих чисел.
```sh
const s = '12,34,56'

const res = s.split(',').reduce((a, e) => a + +e ,0)
console.log(res)
```

### Дана дата в наступному форматі:
'2025-12-31'
#### Преобразуйте эту дату в следующий объект:
```sh
const s = '2025-12-31'


const res = s.split('-')

const object = {
    year: res[0],
    month: res[1],
    day: res[2]
}

console.log(object)
```
#### Дана некоторая строка с буквами и цифрами. Получите позицию первой цифры в этой строке або букви
```sh
onst str = '8768796*/-*/HJGtext45word6lop'
const n = str.search(/\d/);
const n = str.split('').findIndex(e => e >= '0' && e <= '9')
let n2 = -1;
for(let i = 0; i < str.length; i++){
    if(str[i] >= 'A' && str[i] <= 'Z' || str[i] >= 'a' && str[i] <= 'z'){
        n2 = i;
        break;
    }
}
```


### Дано число. Выведите в консоль количество четных цифр в этом числе

```sh
const num = 455578832165;
let n = 0;
const str = num.toString().split('').reduce((a, e) => !(+e % 2) ? a++ : a , 0)
let str = num.toString().split('').reduce((a, e) => !(+e % 2) ? a+1 : a , 0)

for(let i = 0; i < str.length; i++){
    if(!(+str[i] % 2)){
        n++
    }
}
console.log(str)
```
### Дано деякий рядок. Отримайте масив позицій всіх нулів у цьому рядку.
```sh
const str = '023m0df0dfg0';
let arr = [];

// for(let i = 0; i < str.length; i++){
//     if(str[i] === '0'){
//         arr.push(i)
//     }
// }


str.split('').forEach((e, i) => e === '0' && arr.push(i) )

console.log(arr)
```
### Дано деякий рядок. Видаліть кожен третій символ з цього рядка.
```sh
const str = 'abcdefg';
let str2 = '';

for(let i = 0; i < str.length; i++){
    if ((i+1) % 3){
       str2 += str[i]
    }
}

console.log(str2)
```
### Даний деякий масив. Поділіть суму елементів, що стоять на парних позиціях, на суму елементів, що стоять на непарних позиціях.
```sh
const arr = [1, 2, 3, 4, 5, 6];
let par = 0;
let nepar = 0;

// for(let i = 0; i < arr.length; i++){
//     if(!(arr[i] % 2)){
//         par += arr[i]
//     } else {
//         nepar += arr[i]
//     }
// }

arr.forEach(e => (e % 2) === 0 ? par += e : nepar += e)

console.log(par / nepar)
```
### Дано деякий рядок з літерами та цифрами. Отримайте масив позицій усіх цифр із цього рядка.
```sh
const str = 'fds436gg2c5n8';
let arr =  [];

// for(let i = 0; i < str.length; i++){
//     if(str[i] >= '0' && str[i] <= '9'){
//         arr.push(i)
//     }
// }

// str.split('').forEach((e, i) => e >= '0' && e <= '9' && arr.push(i))

const arr2 = str.split('').reduce((a, e, i) => {
    if(e >= '0' && e <= '9'){
         a.push(i)
        console.log(a)
    }
    return a;
}, [])

console.log(arr2)
```
### Даний масив з деякими числами, наприклад, такий:[123, 456, 789] Напишіть код, який переверне числа в цьому масиві за таким принципом: [321, 654, 987]
```sh
const arr = [123, 456, 789];

arr.forEach((e, i) => arr[i] = +e.toString().split('').reverse().join(''))

console.log(arr)
```
### Дано деякий рядок з числом. Відокремте трійки цифр пробілами, починаючи з кінця числа.
```sh
const str = '12245754234567'.split('');
let count = 0;

for(let i = str.length-1; i >= 0; i--){
    count++
    if(count === 3){
        str.splice(i, 0, ' ')
        count = 0
    }
}

console.log(str.join(''))
```
### Змініть регістр букв цього рядка на протилежний. 
```sh
    const str = 'AbCd256*/E';
    let str2 = '';

    for(let i = 0; i < str.length; i++){
        if(str[i] >= 'A' && str[i] <= 'Z'){
        str2 += str[i].toLowerCase()
        } else if(str[i] >= 'a' && str[i] <= 'z') {
            str2 += str[i].toUpperCase()
        } else{
            str2 += str[i]
        }

    }

 const str2 = str.split('').map(e => {
        if(e >= 'A' && e <= 'Z'){
            return e.toLowerCase()
        } else if(e >= 'a' && e <= 'z'){
            return e.toUpperCase()
        }else {
            return e
        }

    })
    .join('')
    console.log(str2)

```
### Даний деякий масив з числами. Злийте пари елементів разом.
```sh
const arr = [1, 2, 3, 4, 5, 6];
let arr2 = [];

for(let i = 0; i < arr.length; i+=2){
        // arr2.push(+(arr[i].toString()+arr[i+1].toString()))
        arr2.push(arr[i]*10 + arr[i+1])
}

console.log(arr2)
```
