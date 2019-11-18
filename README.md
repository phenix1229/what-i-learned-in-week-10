# what-i-learned-in-week-10

## CSS grid

ALternative/complement to flexbox. It is 2 dimensional (row and column at once). 

*Example:*
```
#main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr;
}
```

You can also name the lines/spaces.

*Example:*
```
#main {
    display: grid;
    grid-template-columns: [start] 1fr [middle] 1fr [end];
    grid-template-rows: [start] 1fr [middle] 1fr [end];;
}
```

You can also create grid areas.

*Example:*
```
#app {
  display: grid;
  height: 300px;
  width: 400px;
  grid-template-columns: 1fr 4fr 2fr; 
  grid-template-rows: 1fr 2fr 2fr 1fr;
  grid-template-areas:
  "header header header"
  "nav article-1 ad-area"
  "nav article-2 ad-area"
  "footer footer footer";
}
```

### auto-fit

`grid-template-columns: repeat(auto-fit, minMax(160px, 300px));`

*Exercises:*

https://github.com/phenix1229/japanese-grid-solution

https://github.com/phenix1229/japanese-grid-big

https://github.com/phenix1229/holy-grid-template-areas

---

## Object basics

An object is similar to an array, but is not ordered. It is made of pairs of keys and values.

*Example:*
```
const colin = {
  firstName : 'colin',
  lastName : 'jaffe',
  height : 62,
  age : 39
}
```

2 ways to retrieve data:
  1. console.log(colin['firstName'])
  2. console.log(colin.firstName) - preferred method

2 ways to add keys to an object:
  1. colin['maritalStatus'] = 'married'
  2. colin.maritalStatus = 'married'

You can assign variables based on keys

```
const valueWanted = 'firstName';

console.log(colin[valueWanted])
```

---