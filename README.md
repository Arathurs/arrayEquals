## arrayEquals.js || Simple function to check if two shallow arrays are equal.

#### [Link to Repo](https://github.com/Arathurs/arrayEquals.git/)

### About the Project

This simple function will check to see if two arrays are equal. Note, this method will only work on shallow arrays. 

Testing arrays containing additional nested arrays (or objects) for equality will not work with this function.

### Code

```
function arrayEquals(a,b) {
  return Array.isArray(a) && Array.isArray(b) && a.length === b.length && a.every((val, index) => val === b[index]);
}
```