## forEach
```javascript
let arr = [1, 2, 3, 4]

arr.forEach((a) => {
  console.log(a);
})

/* Output: 
1
2
3
4
*/
```

## map
```javascript
const employees = [
  { id: 20, name: 'Genesis Tadeo' },
  { id: 24, name: 'Jane Joson' },
  { id: 56, name: 'Wesley Juat' },
  { id: 88, name: 'RJ angeles' }
];

const employeeIds = employees.map(employee => employee.id)

console.log(employeeIds)

/* Output:
[ 20, 24, 56, 88 ]
*/
```

## filter
```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

numbers.filter((num) => num % 2 === 0)

/* Output:
[ 2, 4, 6, 8, 10 ]
*/
```

## find

## every & some

## reduce
```javascript
const employees = [
  {
    id: 1,
    name: "Genesis Tadeo",
    years: 2,
  },
  {
    id: 2,
    name: "Jane Joson",
    years: 3
  },
  {
    id: 3,
    name: "Wesley Juat",
    years: 1
  }
]

const totalYears = employees.reduce((accumulator, employee) => {
  return accumulator + employee.years
}, 0)

// console.log(totalYears)

/* Output:
6
*/

const mostExpEmployee = employees.reduce((oldest, employee) => {
  console.log(oldest, employee)
  return (oldest.years || 0) > employee.years ? oldest : employee
})

console.log(mostExpEmployee)

/* Output:
{ id: 2, name: 'Jane Joson', years: 3 }
*/

/*
Example from https://medium.freecodecamp.org/reduce-f47a7da511a9
*/

const fruitBasket = ['banana', 'cherry', 'orange', 'apple', 'cherry', 'orange', 'apple', 'banana', 'cherry', 'orange', 'fig' ];
const count = fruitBasket.reduce( (tally, fruit) => {
  tally[fruit] = (tally[fruit] || 0) + 1 ;
  return tally;
} , {})
count // { banana: 2, cherry: 3, orange: 3, apple: 2, fig: 1 }

fruitBasket.reduce((tally, fruit) => {
  if (!tally[fruit]) {
    tally[fruit] = 1;
  } else {
    tally[fruit] = tally[fruit] + 1;
  }
  return tally;
}, {});
```





