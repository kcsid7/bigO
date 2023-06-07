# Big-O Notation Exercises


#### 1. O(n + 10) 
> O(n)
#### 2. O(100 * n) 
> O(n)
#### 3. O(25) 
> O(1)
#### 4. O(n^2 + n^3) 
> O(n^3)
#### 5. O(n + n + n + n)
> O(n)
#### 6. O(1000 * log(n) + n)
> O(n)
#### 7. O(1000 * n * log(n) + n) 
> O(nlog(n))
#### 8. O(2^n + n^2)
> O(n^2)
#### 9. O(5 + 3 + 1) 
> O(1)
#### 10. O(n + n^(1/2) + n^2 + n * log(n)^10)
> O(n^2)

#### 11. O(n)
```Javascript
function logUpTo(n) {
  for (let i = 1; i <= n; i++) {
    console.log(i);
  }
}
```

#### 12. O(n)
```Javascript
function logAtLeast10(n) {
  for (let i = 1; i <= Math.max(n, 10); i++) {
    console.log(i);
  }
}
```

#### 13. O(1)
```Javascript
function logAtMost10(n) {
  for (let i = 1; i <= Math.min(n, 10); i++) {
    console.log(i);
  }
}
```

#### 14. O(n)
```Javascript
function onlyElementsAtEvenIndex(array) {
  let newArray = [];
  for (let i = 0; i < array.length; i++) {
    if (i % 2 === 0) {
      newArray.push(array[i]);
    }
  }
  return newArray;
}
```

#### 15. O(n^2)
```Javascript
function subtotals(array) {
  let subtotalArray = [];
  for (let i = 0; i < array.length; i++) {
    let subtotal = 0;
    for (let j = 0; j <= i; j++) {
      subtotal += array[j];
    }
    subtotalArray.push(subtotal);
  }
  return subtotalArray;
}
```

#### 16. O(n)
```Javascript
function vowelCount(str) {
  let vowelCount = {};
  const vowels = "aeiouAEIOU";

  for (let char of str) {
    if(vowels.includes(char)) {
      if(char in vowelCount) {
        vowelCount[char] += 1;
      } else {
        vowelCount[char] = 1;
      }
    }
  }

  return vowelCount;
}
```



#### 17. True or false: n^2 + n is O(n^2).
> True
#### 18. True or false: n^2 * n is O(n^3).
> True
#### 19. True or false: n^2 + n is O(n).
> False
#### 20. What’s the time complexity of the .indexOf array method?
> O(n)
#### 21. What’s the time complexity of the .includes array method?
> O(n)
#### 22. What’s the time complexity of the .forEach array method?
> O(n)
#### 23. What’s the time complexity of the .sort array method?
> O(nlog(n))
#### 24.  What’s the time complexity of the .unshift array method?
> O(n)
#### 25. What’s the time complexity of the .push array method?
> O(1)
#### 26. What’s the time complexity of the .splice array method?
> O(n)
#### 27. What’s the time complexity of the .pop array method?
> O(1)
#### 28. What’s the time complexity of the Object.keys() function?
> O(n)


