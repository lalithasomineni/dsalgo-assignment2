# using iteration

```
function fib(n){
  let arr = [0, 1];
  for (let i = 2; i < n + 1; i++){
    arr.push(arr[i - 2] + arr[i -1])
  }
 return arr[n]
}
//fib(12)

```

```
function reverse(string){
  let reversed = "";    
  for (var i = string.length - 1; i >= 0; i--){        
    reversed += string[i];
  }    
  return reversed;
}

//reverse("lalli");
```

```
function factorial(n){
  let answer = 1;
  if (n == 0 || n == 1){
    return answer;
  }else{
    for(var i = n; i >= 1; i--){
      answer = answer * i;
    }
    return answer;
  }  
}

//factorial(4);

```
```
function palindrome(string) {
 var length = string.length;
 for (var i = 0; i < length/2; i++) {
   if (string[i] !== string[length - 1 - i]) {
       return false;
   }
 }
 return true;
}
//palindrome("lalli");

```


```
function prime_factors(num) {
  function is_prime(num) {
    for (let i = 2; i <= Math.sqrt(num); i++)
    {
      if (num % i === 0) return false;
    }
    return true;
  }
  const result = [];
  for (let i = 2; i <= num; i++)
  {
    while (is_prime(i) && num % i === 0) 
    {
      if (!result.includes(i)) result.push(i);
      num /= i;
    }
  }
  return result;
}
//console.log(prime_factors(100));

```
# using recursion

```
function factorialize(number) {
  if (number < 0) 
        return -1;
  else if (number == 0) 
      return 1;
  else {
      return (number * factorialize(number - 1));
  }
}
//factorialize(5);

```
```
function reverseString(str) {
  if (str === "")
    return "";
  else
    return reverseString(str.substr(1)) + str.charAt(0);
}
//reverseString("hello");

```
```
function test_prime(n)
{

  if (n===1)
  {
    return false;
  }
  else if(n === 2)
  {
    return true;
  }else
  {
    for(var x = 2; x < n; x++)
    {
      if(n % x === 0)
      {
        return false;
      }
    }
    return true;  
  }
}

//console.log(test_prime(37));

```
```

function fib(n){
  if(n < 2) return n;
  
  return (n - 1) + (n - 2);
}

fib(10);

```
