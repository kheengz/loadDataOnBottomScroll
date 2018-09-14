##ReactJS

### Auto Load data on bottom scroll of page

##### A React code for auto loading more contents on scrolling to the bottom aspect of a container/page
- Displays 12 boxes 6 on each rows on initial load 
- On 1st bottom scroll, displays loading gif icon and waits for 2000ms, then loads more 6 boxes total boxes now 18
- On 2nd bottom scroll, displays loading gif icon and waits for 2000ms, then loads more 6 boxes total boxes now 24
- On 3rd bottom scroll, displays loading gif icon and waits for 2000ms, then loads more 6 boxes total boxes now 30

> The boxes are loading not to infinite due to a controlled condition called `loadedAllData` which is a boolean and `false` as default

> `loadedAllData` controls when the total/exhausted data are loaded, in this case we only needed to load 30 boxes.

> setting the state `loadedAllData: newData.length >= 29` where `29 === (30 - 1)`,
 
> as soon as `loadedAllData` becomes `true`, the data stops loading new record even if the page scroll is at the bottom.


