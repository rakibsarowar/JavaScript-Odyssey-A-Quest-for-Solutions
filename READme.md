Problem list:
 - [1. Reversing a String](#1-Reversing-a-String)
 - [2. Finding the Largest Number in an Array](#2-Finding-the-Largest-Number-in-an-Array)
 - [3. Checking for Palindromes](#3-Checking-for-Palindromes)
 - [4. Counting the Number of Words in a Sentence](#4-Counting-the-Number-of-Words-in-a-Sentence)
 - [5. Removing Duplicates from an Array](#5-Removing-Duplicates-from-an-Array)
   



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
