[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/GDPVb20V)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
// The mystery() function finds the greatest value in an array. It first checks for the base case, if the array consists of only one element. If so, it is by default the largest element in the array 
// so it returns the first and only element. If not, the function recursively calls passing a.slice as the array. This creates a new array with elements starting at element 1 till the last element. 
// This will recurse until the array has only one element, which is the last element of the original array. It will then be assigned to foo, and compared to the first element. It will return whichever is greater
// in value. This passes all the way up till the first call of the function where it compares foo, and the first element and returns whatever is greater. 
