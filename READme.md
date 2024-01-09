Problem list:
 - [1. Reversing a String](#1-Reversing-a-String)
 - [2. Finding the Largest Number in an Array](#2-Finding-the-Largest-Number-in-an-Array)
 - [3. Checking for Palindromes](#3-Checking-for-Palindromes)
 - [4. Counting the Number of Words in a Sentence](#4-Counting-the-Number-of-Words-in-a-Sentence)
 - [5. Removing Duplicates from an Array](#5-Removing-Duplicates-from-an-Array)
 - [6. Marge two arrey and remove duplicates from the arey](#6-Marge-two-arrey-and-remove-duplicates-from-the-arey)
 - [7. What are the final values of a and b after executing the following code in JavaScript?](#7-what-are-the-final-values-of-a-and-b-after-executing-the-following-code-in-javascript)
   

## 1. Reversing a String
Problem: Write a function that reverses a given string.
<br>

```
function reverseString(str) {
  return str.split('').reverse().join('');
}

// Example usage
console.log(reverseString('hello')); // Output: 'olleh'

Way 2:
const reverseString = str => {
  return str.split("").reverse().join("");
}

console.log(reverseString("rakib")); // Output: 'bikar'

```
<br>

```

Way 3: 
const reverseString = str => str.split("").reverse().join("");

console.log(reverseString("rakib")); // Output: 'bikar'

```

## 2. Finding the Largest Number in an Array
Problem: Write a function that finds the largest number in an array.
<br>

```
function findLargestNumber(arr) {
  return Math.max(...arr);
}
// Example usage
console.log(findLargestNumber([3, 9, 1, 25, 7])); // Output: 25


findLargestNumber = arr => Math.max(...arr)


console.log(findLargestNumber([3,4,5,6,69]))

```
<br>

## 3. Checking for Palindromes
Problem: Create a function that checks whether a string is a palindrome.
<br>

```
Way 1:
function isPalindrome (str) {
  const reverse = str.split('').reverse().join("");
  return str === reverse
}
console.log(isPalindrome("rakib"))


Way 02: 
isPalindrome = str => {
  const reverse = str.split('').reverse().join("")
  return str === reverse
}
console.log(isPalindrome("lol"))
// Output: false

```


## 4. Counting the Number of Words in a Sentence
Problem: Write a function that counts the number of words in a given sentence.
<br>

```
function count (sentence) {
  const words = sentence.split("").filter(word => word.trim() !== "")
  return words.length
}


console.log(count("i love you"))


const count = sentence => {
  const words = sentence.split("").filter(word=> word.trim() !=="")
  return words.length
} 


console.log(count("i love you"))

```
<br>

## 5. Removing Duplicates from an Array
Problem: Write a function that can remove duplicates from an array. <br>
<br>

```
//Way01:

function removeDuplicates(arr) {
  return [...new Set(arr)];
}

// Example usage:
const array = [1, 2, 2, 3, 4, 4, 5];
console.log(removeDuplicates(array)); // Output: [1, 2, 3, 4, 5]

```

```
//Way02:
const array = [1, 2, 2, 3, 4, 4, 5];
removeDuplicates = array => [...new Set(array)]
console.log(removeDuplicates(array)); // Output: [1, 2, 3, 4, 5]
```

# 6. Marge two arrey and remove duplicates from the arey. 

```
A = [1,2,2,3,,4,5,5]
B = [6,7,8,9]
const AB=A.concat(B)
const newArrey = [...new Set(AB)]
console.log(newArrey)
```
## 7. What are the final values of a and b after executing the following code in JavaScript?

```
let a = 5;
let b = a++;
console.log(a, b);
```
Solution:
1.	`let a = 5;` - It declares a variable a and assigns it the value 5. <br>
2.	`let b = a++;` - This line has two parts:
•	`a++` is a post-increment operation. `a++` means that the current value of `a` (which is `5`) is assigned to `b`, and then `a` is incremented by `1`. <br>
•	So, after this line executes, b holds the value 5 because the current value of `a` (before incrementing) is assigned to `b`, and `a` gets incremented to `6`. <br>
3.	`console.log(a, b);` - This prints the values of `a` and `b` to the console. <br>
•	`a` now holds the value 6 because it was incremented after the assignment to `b`.
•	`b` holds the original value of `a`, which is `5`. <br>
Therefore, when you execute `console.log(a, b);`, it will output `6, 5`.

```
let a = 5;
let b = a; // Assign the current value of 'a' to 'b'
a = a + 1; // Increment 'a' by 1
```
