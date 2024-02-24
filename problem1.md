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
