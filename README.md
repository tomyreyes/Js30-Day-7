This repo refers to **Day 7** of the **JavaScript 30 for 30** challenge https://javascript30.com/

In today's challenge I worked with and learned more array prototypes that will be useful for making clean code in the future.

**What I learned**

array.prototype.some() - 

this method tests whether at least one element in an array meets a condition created by a function. This returns a boolean.
Example:

```
const pets = ['cat', 'dog', 'goldfish', 'parrot']; 

function checkPet(array, value) {
  return array.some(arrayValue => value === arrayValue); 
}

checkPet(pets, 'frog'); //false
checkPet(pets, 'dog'); //true
```

array.prototype.every() - 

this method is similar to .some(), where it differentiates is that it will test whether **all** elements in an array pass a test created by a function. 
Example:

```
[1,2,3,4,5,6,7,8].every(x => x <10); 
```

array.prototype.find() - 

this method will return the first element it finds that meets the conditions provided by a function. 
Example:

```
const array = [6, 5, 12, 4, 7];

function overTen (element){
  return element >=10; 
}

array.find(overTen); //12 
```

.findIndex() 

this method is similar to .find() but as the name suggests, it will return the index of the first element that meets the conditions provided by a function. 
Example:

```
const randoNums = [11, 5, 25, 79, 1001, 112, 6, 9, 67];
function findFavNum(element) {
  return element ===6;
}
randoNums.findIndex(findFavNum); //6
```
