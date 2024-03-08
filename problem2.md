### провірка чи є строка полідромом
```sh
const str = 'aba';

const str2 = str.split('').reverse().join('');
console.log(str)
console.log(str2)
if(str === str2){
    console.log('string polidrom')
} else {
    console.log('string not polidrom')
}
```
