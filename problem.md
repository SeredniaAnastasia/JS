### Провірка на відємне число

<details><summary>Рішення</summary>
```sh
const isMinus =(n) => n < 0 ? true : false
```
</details>

### Повернути останній символ з строки
```sh
Варіант 1
const getLaterSymbol =(str) => str[ str.length-1 ]
Варіант 2
const getLaterSymbol =(str) => str.at(-1)
```

### Провірка на парне число
```sh
 Варіант 1
 const isEven =(n) => !!(n % 2)
 Варіант 2
 const isEven =(n) => n % 2 === 0
```
### Провірка перших літер в двох словах
```sh
const isFirstLater =(str1, str2) => str1[0] === str2[0];
```

### Дане слово. Отримайте останню літеру. Якщо слово закінчується на м'який знак, отримайте передостанню букву.
```sh
const getLaterSymbol =(str1) => str1.at(-1) === 'ь' ? str1.at(-2) : str1.at(-1)
```

### Дано число. Виведіть у консоль першу цифру цього числа.
```sh
const getFirstNumber =(num) => num.toString()[0]
```
### Дано число. Виведіть у консоль останню цифру цього числа.
```sh
const getLastNumber =(num) => num.toString().at(-1)
```
### Дано число. Виведіть у консоль суму першої та останньої цифри цього числа.
```sh
const getSumFirstAndLastNumber = (num) => +num.toString()[0] + +num.toString().at(-1)
```
### Дано число. Виведіть кількість цифр у цьому числі.
```sh
const getLengthNumber= (num) => num.toString().length
```
### Дано два числа. Перевірте, чи перші цифри цих чисел збігаються.
```sh
const isFirstNumber= (num1, num2) => num1.toString()[0] === num2.toString()[0]
```

### Дано рядок. Якщо в цьому рядку більше одного символу, виведіть передостанній символ цього рядка в консоль.
```sh
const getBeforeTheLastNumber = (str) => str.length > 0 ? str.at(-2) : undefined 
```

### Дано два цілих числа. Перевірте, що перше число без залишку поділяється на друге.
```sh
const isDivisionWithoutRemainder = (num1, num2) => !(num1 % num2) 
```

### Виведіть у консоль усі парні числа із проміжку від 1 до 100.
```sh
const printWholeNumbers = () => {
    for(let i=1; i<=100; i++){
        !(i % 2) && console.log(i)
    }
}
```

### Повернути в обєкті окркмо суму парних і непарних чисел 
```sh
const getSumNumber = () => {
    let sumOfEvenNumbers = 0;
    let sumOfOddNumbers = 0;
    for(let i=1; i<=100; i++){
        if(!(i % 2))
        sumOfEvenNumbers += i;
        else
        sumOfOddNumbers += i;
    }
    return {
      sumOfEvenNumbers,
      sumOfOddNumbers
    }
}
```

### Даний масив із числами. Знайдіть суму квадратів елементів цього масиву.
```sh
const arr =  [10, 22, 8, 3, 7, 67, 34, 345, 34, 12];
let sum =0;
for(let i = 0; i < arr.length; i++){
    sum+= arr[i]**2;

}

arr.forEach(e => sum += e**2)
const summa = arr.reduce((a, e) => {
   return a + e**2
}, 0)

console.log(summa)
```
### Округліть ці дроби до одного знака в дрібній частині.
```sh
const m = [1.456, 2.125, 3.32, 4.1, 5.34]; 

function roundingNumber(arr){
    const m2 = []
    arr.forEach(e => {
        m2.push(Number.parseFloat(e.toFixed(1)))
    })
    return m2
}

function roundingNumber(arr){
  return arr.map(e => Number.parseFloat(e.toFixed(1)));
}

console.log(roundingNumber(m))
```
### Дано масив з рядками. Залишіть у цьому масиві лише ті рядки, які починаються на http://.
```sh
const arrStr = [
    'http://.google.com',
    'http://.youtube.com',
    'yandex http://.yandex.ru ',
    'codemu http://.code.mu'
]
const arr = [];
for(let i= 0; i < arrStr.length; i++){
    if(arrStr[i].indexOf('http://') === 0){
        arr.push(arrStr[i])
    }
}
console.log(arr)
```
