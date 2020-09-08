# Arrays
Recall that there are three data types:
- Numeric: `4`
- String: `'Hello'`
- Boolean: `true` or `false`

And data can be stored in variables:

```
var count = 4;
var message = 'Hello';
var isTheSunUp = true;
```
Write shorter code like this:

```
var count = 4, message = 'Hello', isTheSunUp = true;
```

To make a list of data, you'll need to create an *array*.

```
var iowaCities;
iowaCities = ['Des Moines', 
              'Cedar Rapids',
              'Iowa City'];
```
The number each item is assigned to in the array list is called an **index**, and it starts the count from 0.

Index | Value
-----|-----
0 | `'Des Moines'`
1 | `'Cedar Rapids'`
2 | `'Iowa City'`

We can use the **index** to access or change items in an array.
``` 
var iowaCities;
iowaCities = ['Des Moines', 
              'Cedar Rapids',
              'Iowa City'];

// Change the third city in the list to 'Ames'
iowaCities[2] = 'Ames'

// Assign variable cycloneCity to the third value in the array
var cycloneCity = iowaCities[2]
```