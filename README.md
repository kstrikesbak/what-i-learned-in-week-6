# **WHAT I LEARNED IN  WEEK 6** 
___

## `Whiles and Numbers All Wrapped Up In Strings`


```javascript
function challengeBanner (num) {
  console.log('######### Challenge ' + num + ' #########');
}

challengeBanner(1);

function count5() {
  let i = 1;
  while(i<=5){
    console.log(i)
    i=i+1;
  }
}

count5();

challengeBanner(2);

function oneToWhatever(n) {
  let i = 1;
  while(i<=n) {
    console.log(i)
    i=i+1;
  }
}

oneToWhatever(6);

challengeBanner(3);

function printsFirstToSecond(a,b) {
  let i = a;
  while(i<=b) {
    console.log(i)
    i=i+1;
  }
}

printsFirstToSecond(5,14);

challengeBanner(4);

function printsNumAndtype (n) {
  let i =1;
  while(i<=n) {
   
  if (i%2===0) {
    console.log(i +' EVEN')
  } else {
    console.log( i +' ODD')
  }
  i=i+1;
  
  }
}

printsNumAndtype(5);

challengeBanner(5);

function printEvenNumbers(n) {
  let i=2; 
  while(i<=n) {
    if (i%2===0) {
      console.log(i)
    }
    i=i+1;
  }
}

printEvenNumbers(10);

challengeBanner(6);


function descendingOrder(n) {
  let i=n;
  while (i>0) {
    console.log(i)
    i=i-1
  }
}

descendingOrder(10);

challengeBanner(7);

function descendingOrderAndBlastOff(n) {
  let i=n;
  while (i>0) {
    console.log(i)
    i=i-1
  } if (i=1) {
    console.log('Blast off!');
  }
}

descendingOrderAndBlastOff(10);

challengeBanner(8);

function printsFromParameterDownTo1 (n) {
  let i=n;
  while(i>=1) {
    console.log(i)
    i=i-3
  }
}

printsFromParameterDownTo1(20);

challengeBanner(9);

function printsHelloSevenTimesAndNumber (n) {
  let i = 1;
  while (i<n) { 
    console.log('Hello. ' + i)
    i=i+1;
  }
}

printsHelloSevenTimesAndNumber(8);

challengeBanner(10);

function printStrMultipleTimes (n) {
  let i = 0;
  while (i<n) { 
    console.log("Cheese")
    i=i+1;
  }
}

printStrMultipleTimes(7);

challengeBanner(11);

function printsHelloSevenTimesWithStr (str,n) {
  let i = 1;
  while (i<n+1) { 
    console.log(str + i)
    i=i+1;
  }
}

printsHelloSevenTimesWithStr("Good-bye...",4);

challengeBanner(12);

function takesInStrAndPrintsEveryCharacter(str) {
  let i=0;
  while (i<str.length) {
    console.log(str[i])
    i=i+1;
  }
  
}

takesInStrAndPrintsEveryCharacter('think');

challengeBanner(13);

function everySecondCharacter(str) {
  let i=-1;
  while (i<str.length) {
    console.log(str[i])
    i=i+2;
  }
}

everySecondCharacter("Nobody");

challengeBanner(14);

function printsAStringBackwards (str) {
  let i=str.length-1;
  while (i>=0) {
    console.log(str[i])
    i=i-1;
  }
}

printsAStringBackwards("HELLO")

challengeBanner(15);

function takesInANumberAndPrintsEachIntegerFrom1ToThatNumber (n) {
  let i=1;
  while (i<=n) {
    if (i%3 === 0) {
    console.log("Fizz");
  } else if (i%5 === 0) {
    console.log("Buzz");
  } else if (i%15===0) {
    console.log("FizzBuzz");
  }
  else {
      console.log(i);
    } 
    i=i+1;
  }
}


takesInANumberAndPrintsEachIntegerFrom1ToThatNumber(15);

challengeBanner(16);




```
___

## `String Loops`

```javascript
function acceptsANumberAndPrintsOutABanner (n) {
  console.log(`##### Challenge ${n} #####`);
}

acceptsANumberAndPrintsOutABanner(1);

function printsOutOnlyVowels (str) {
  let i=0
  while(i<=str.length) {
    if (str[i]==='a') {
      console.log('a')
    } else if (str[i]==='e') {
      console.log('e')
    } else if (str[i]==='i'){
      console.log('i')
    } else if (str[i]==='o'){
      console.log('o')
    } else if (str[i]==='u'){
      console.log('u');
  } i = i + 1;
}
}
printsOutOnlyVowels ("Regular expressions are for term 2.")

// function first5Vowels(str){
// let i = 0;
// while( i <= str.length){
//   if (str[i] === 'a' || str[i] === 'e' || str[i] === 'i' || str[i] === 'o' || str[i] === 'u'){
//     console.log(str[i])
//   }
//       i = i + 1
//   }
// }
// first5Vowels('kejal')

acceptsANumberAndPrintsOutABanner(2);

function first5Vowels(str){
 let i = 0;
 let countVowels = 0
 while( i <= str.length){
   if (str[i] === 'a' || str[i] === 'e' || str[i] === 'i' || str[i] === 'o' || str[i] === 'u'){
     console.log(str[i])
     countVowels = countVowels + 1
   }
   if (countVowels === 5){
     break
   }
      i = i + 1;
 }
}
first5Vowels('Regular expressions are for term 2.')

acceptsANumberAndPrintsOutABanner(3);

function printsOutEveryThirdCharacter (str) {
  let i = 2;
  while(i<=str.length) {
    console.log(str[i])
  i=i+3
  }
}

printsOutEveryThirdCharacter("I am the alfalfa and the omelette.")

acceptsANumberAndPrintsOutABanner(4);

function printsOutFirstFourCharactersAfterGivenIndex(str,n) {
  let i=n;
  while(i<=n+3) {
    console.log(str[i])
  i=i+1;
  }
}

printsOutFirstFourCharactersAfterGivenIndex("Oh hi, I didn't see you there. Welcome.",4)

acceptsANumberAndPrintsOutABanner(5);

function printsOutEveryU (str) {
  let i=0;
  while(i<=str.length) {
    if (str[i] === 'u') {
    console.log(i)
    }
    i=i+1;
  }
}

printsOutEveryU ('You picked the wrong house, bub.')


acceptsANumberAndPrintsOutABanner(6);


function printsOutFirstU (str) {
  let i=0;
  let uCount = 0;
  while(i<=str.length) {
    if (str[i] === 'u') {
    console.log(i)
    uCount = uCount + 1
    if(uCount===1) {
      break;
    }
    }
    i=i+1;
  }
}


printsOutFirstU ('You picked the wrong house, bub.')


// function onlyU2(str){
// let i = 0
// let countU = 0
// while (i<= str.length ){
//   if (str[i]=== 'u'){
//   console.log(i)
//   countU = countU + 1
//   if(countU === 1){
//   break;
//   }
//   }
//   i = i + 1
// }
// }
// onlyU2 ('You picked the wrong house, bub.');

acceptsANumberAndPrintsOutABanner(7);
  
function printsOutTheFirstIndexOfTheLetterU(str){
 let i = 0
 let countU = 0
 while (i<= str.length ){
   if (str[i]=== 'u'){
   console.log(i)
   countU = countU + 1
     if(countU === 1){
       break;
     }
   }
   i = i + 1
 }
 if(countU === 0){
   console.log(-1)
 }
}

printsOutTheFirstIndexOfTheLetterU ("I'm Canadian.")
printsOutTheFirstIndexOfTheLetterU ('You picked the wrong house, bub.')


```

## `You Deserve Arrays`

This was a great introduction to arrays. 

```javascript
function getFirstItemFrom(arr) {
return arr[0]
}


function getLastItemFrom(arr) {
return arr[arr.length -1]
}

function getIndex3(arr) {
if (arr.length >3) {
return arr[3]
} else {
  return arr[arr.length-1];
}
}

function firstItemIsNumber(arr) {
  return typeof arr[0] === 'number'
}


function isLongList(arr) {
return arr.length>9
}

```

## `Array of radioactive mutants`



```javascript
function changeLast(arr,num) {
  arr[arr.length-1] = num;
}
const arr1 = [1, 2, 3];
const arr2 = [1, 2];
changeLast(arr1,5);
changeLast(arr2,5);

function addMeToEnd(arr) {
  arr.push("Colin")
}

addMeToEnd(arr1)
addMeToEnd(arr2)

function addMeToStart(arr) {
  arr.unshift("Colin")
}

addMeToStart(arr1)
addMeToStart(arr2)

function changeAllValuesTo(arr,value) {
  let i=0
  while (i< arr.length) {
  arr[i]= value;
  i++
  }
}
changeAllValuesTo(arr1,15)
changeAllValuesTo(arr2,30)

function oddOrEven(arr) {
  let i=0
  while (i< arr.length) {
    if (arr[i] % 2 === 0) {
      arr[i] = 'even'
    } else {
      arr[i] = 'odd'
    }
  
  i++
  }
}
oddOrEven(arr1);
oddOrEven(arr2);

function changeNextThreeToValue(a,arr,b) {
  let i=a;
  while (i<a+3) {
    arr[i] = b
    i++
  }
}


changeNextThreeToValue(2,arr1,15)
changeNextThreeToValue(1,arr2,15)

module.exports = {
  changeLast,
  addMeToEnd,
  addMeToStart,
  changeAllValuesTo,
  oddOrEven,
  changeNextThreeToValue,
}
```