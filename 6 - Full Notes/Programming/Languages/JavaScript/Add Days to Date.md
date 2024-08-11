
2024-08-10 22:17

Tags: [[JavaScript]]

### Overview
Manipulating dates in [[JavaScript]] is something you need to do often.

To add a certain number of days to a JavaScript `Date` (or string) you need to do the following:

### Steps
1. Convert the string to a `Date` object
2. Use the `.setDate()` function with the sum of `getDate()` and `days` you want to add.


### Code
```javascript

const addDays = (startDate, daysToAdd) => {
    const newDate = new Date(startDate);
    return newDate.setDate(newDate.getDate() + daysToAdd);
}

const startDate = new Date("2024-08-10");
const endDate = addDays(startDate, 5);

console.log(startDate.toDateString());
// Fri Aug 09 2024

console.log(endDate.toDateString());
// Wed Aug 14 2024

```
