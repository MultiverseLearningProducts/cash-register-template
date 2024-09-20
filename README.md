# Cash Register Project

# Activity Directions

**GOAL**: In `index.js`, there are a collection of functions which provide functionality for a cash register to be used by a point-of-sale system. Your task is to complete the functions by writing the logic to meet the specifications below:

- **Level 1**:
  - `removeItem(name, drawer)`: Removes a single item from the drawer
  - `addItem(name, drawer)`: Adds a single item to the drawer
- **Level 2**:
  - `countCoins(drawer)`: Counts how many coins are in the drawer
  - `countNotes(drawer)`: Counts how many notes/bills are in the drawer
- **Level 3**:
  - `sumDrawer(drawer)`: Calculates the total amount of money in the drawer as a string formatted in dollars (see example below)
- **Level 4**:
  - `canMakeAmount(target, drawer)`: Determines whether it is possible to create a specific cash amount from the items in the drawer.
- **Level 5**:
  - `transaction(cost, paid, drawer)`: Calculates the change required from a transaction and removes it from the drawer if possible.

Each function accepts a `drawer` array of objects. Currency types and amounts that may be in the `drawer` array are [represented in integers rather than decimals](https://blog.agentrisk.com/you-better-work-in-cents-not-dollars-2edb52cdf308).

| Currency Unit       | Amount |
| ------------------- | ------ |
| Penny               | 1      |
| Nickel              | 5      |
| Dime                | 10     |
| Quarter             | 25     |
| Dollar              | 100    |
| Five Dollars        | 500    |
| Ten Dollars         | 1000   |
| Twenty Dollars      | 2000   |
| One-hundred Dollars | 10000  |

An example `drawer` array of objects has been provided for you in the `drawer.js` file.

```javascript
const drawer = [
  { name: "penny", value: 1, quantity: 72 },
  { name: "nickel", value: 5, quantity: 41 },
  { name: "dime", value: 10, quantity: 31 },
  { name: "quarter", value: 25, quantity: 17 },
  { name: "one", value: 100, quantity: 90 },
  { name: "five", value: 500, quantity: 11 },
  { name: "ten", value: 1_000, quantity: 2 },
  { name: "twenty", value: 2_000, quantity: 3 },
  { name: "hundred", value: 10_000, quantity: 1 },
];
```

### Running and Testing Your Code

1. Run your code (`npm start`).
2. Test your code (`npm test`).
