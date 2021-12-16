1. Using loops take 10 inputs from user and find the average of all the numbers.

function average(num1,num2,num3,num4,num5,num6,num7,num8,num9,num10){
  return (num1 + num2 + num3 + num4 + num5 + num6 + num7 + num8 + num9 + num10)/10;
}

average(1,2,3,4,5,6,7,8,9,10);

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```

-- 'hi'
'hi'
'hi'

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

function getEvenSum(max=10){
let sum =0;
for(i=1;i<=max;i++){
  if(i%2==0){
    sum+=i
  }
}
return sum;
}

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

function getOddSum(max=10){
let sum =0;
for(i=1;i<=max;i++){
  if(i%2!=0){
    sum+=i
  }
}
return sum;
}

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

function getProductOfDigits(num){
  if(num>0){
  let numToStr = num.toString()
  let product = 1;
  for(let i = 0; i < numToStr.length; i++){
    product *= Number(numToStr[i])
  }
  return product
  }else{
    return  `not a valid input`
  }
}

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // output -- Bigger than 5
check(1); // output - Smaller than 5
check(5); // output - 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // what will be the output - You are arya
getOutput('John'); // what will be the output - You are John
getOutput(); // what will be the output - 'Who are you'
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // what will be the output - undefined
getOutput('John'); // what will be the output - undefined
getOutput(); // what will be the output - 'Who are you'
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

yes

function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}


10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

if you know the start and end number to loop then it is better to go for for loop, other =wise we will go for while.

sum of 1-10

let sum =0;

for(i=1;i<=10;i++){
  sum+=i
  returnn sum;
}

Iterating through array

let arr = [1,2,3,4]

let i=0;

while(arr[i]==3){
  i++
}
