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
### Дан некоторый массив, например, вот такой:
[1, 2, 3, 4, 5, 6]
#### Поделите сумму первой половины элементов этого массива на сумму второй половины элементов.
```sh
arr.forEach((e, i, arr)=>{
    if(arr.length /2 > i)
        sum1 += e;
    else
        sum2 += e;
})
```
