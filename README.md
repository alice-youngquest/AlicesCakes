# AlicesProject
- give a brief description of the Box Model

Its essentially a box which goes around each HTML element. It includes margins, borders, padding, and your content. By treating each element on the page as a box it helps us apply different properties that allow us to define where that element sits of the web page.

1. Return the sum of the price of all properties as a single value

//create new array of all price values
const priceArray = sales.map(element => element.price);
console.log(priceArray);

//take that new array and add each number together.
 the zero is there to ensure a number if the array was empty.
var sumOfPrice = priceArray.reduce(function(a, b){
        return a + b;
    }, 0);

// total sum 469.85999999999996
console.log(sumOfPrice)

2. Return the items which were sold in 2017.

//first day of 2017 & last day
const startDate = "2017-01-1"
const endDate = "2017-12-31"

// filter on sales only returning dates between my variables
result = sales.filter(d => {var date = d.dateSold;
        return (startDate <= date && date <= endDate);
    });
console.log(result);


3. Return an array of all of the itemsSold properties as strings, sorted alphabetically

//creating a new array with the property itemSold and a sort to order it alphabetically. if they were numbers i would have had to use .sort(function(a, b){return a - b}).

const sortedItems = sales.map(element => element.itemSold).sort();
console.log(sortedItems);

4. the question didn't really make sense to me i'm not sure if thats my brain being funny and not interpreting it right. So i decided to leave it and move on.


My webpage.

i decided to focus on a minimalist design otherwise there was a fair possibility i would never hand this in cause i like things to look perfect. but im happy with the way the photos react to the resizing of the browser. i tried sticking to the block element modifier naming methodology.

things i wanted to do if i gave myself more time:

- better use of the scss variables and mixins.  
 (i think this was at fault of me not having much on the screen)
- id probably fix the header bar so it didnt scroll with the page, i think its handy to always be able to reach it.
- Id also create a better git workflow - apparently it isnt like riding a bike and i was having trouble remembering the flow of it again and the commands (i feel like i could have easily spent a day or so getting use to this again). so thats also something i have put aside as i didnt want to spend a crazy amount of time on this.
but if i had used it properly i probably would have branched off for each piece of work e.g sideBar, header, content area. and then maybe each block in the respective areas. i feel like those would have been good places to checkin.
