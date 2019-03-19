## Callback Function
```javascript
setTimeout(() => {
  console.log('Two seconds are up')
}, 2000)

const geocode = (address, callback) => {
  setTimeout(() => {
    const data = {
      latitude: 0,
      longitude: 0
    }
    callback(data)
  }, 2000)
}

geocode('Philadelphia', (data) => {
  console.log(data)
})

const add = (a, b, callback) => {
  setTimeout(() => {
    const sum = a + b
    callback(sum)
  }, 2000)
}

add(1, 4, (sum) => {
  console.log(sum)
})

add(2, 5, (sum) => {
  console.log(sum)
})

/* Output:
Two seconds are up
{ latitude: 0, longitude: 0 }
5
7
*/
```