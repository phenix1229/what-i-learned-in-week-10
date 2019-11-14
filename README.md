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
*Exercises:*

https://github.com/phenix1229/japanese-grid-solution

https://github.com/phenix1229/japanese-grid-big

https://github.com/phenix1229/holy-grid-template-areas