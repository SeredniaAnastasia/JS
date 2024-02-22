## Провірка на відємне число
```sh
const isMinus =(n) => n < 0 ? true : false
```
## Повернути останній символ з строки
```sh
Варіант 1
const getLaterSymbol =(str) => str[ str.length-1 ]
Варіант 2
const getLaterSymbol =(str) => str.at(-1)
```

## Провірка на парне число
```sh
 Варіант 1
 const isEven =(n) => !!(n % 2)
 Варіант 2
 const isEven =(n) => n % 2 === 0
```
## Провірка перших літер в двох словах
```sh
const isFirstLater =(str1, str2) => str1[0] === str2[0];
```

## Дане слово. Отримайте останню літеру. Якщо слово закінчується на м'який знак, отримайте передостанню букву.
```sh
const getLaterSymbol =(str1) => str1.at(-1) === 'ь' ? str1.at(-2) : str1.at(-1)
```

## Дано число. Виведіть у консоль першу цифру цього числа.
```sh
const getFirstNumber =(num) => num.toString()[0]
```
## Дано число. Виведіть у консоль останню цифру цього числа.
```sh
const getLastNumber =(num) => num.toString().at(-1)
```
