### Object property shorthand
```javascript
const name = 'Genesis'
const userAge = 26

const user = {
  name,
  age: userAge,
  location: 'Pasay'
}

console.log(user)

/* Output:
{ name: 'Genesis', age: 26, location: 'Pasay' }
*/
```

### Object destructuring
```javascript
const product = {
  label: 'Box',
  price: 5,
  stock: 220,
  salePrice: undefined,
  rating: 4.6
}

// const label = product.label
// const stock = product.stock

// const {label:productLabel, stock, rating = 5} = product
// console.log(productLabel)
// console.log(stock)
// console.log(rating)

const transaction = (type, { label, stock = 0 } = {}) => {
  console.log(type, label, stock)
}

transaction('order', product)
/* Output:
order Box 220
*/

```
