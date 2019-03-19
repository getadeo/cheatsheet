### Javascript client side HTTP request
```javascript
fetch('https://httpbin.org/get?name=getadeo').then((response) => {
  response.json().then((data) => {
    console.log(data.args.name)
  })
})

/* Output:
getadeo
*/
```