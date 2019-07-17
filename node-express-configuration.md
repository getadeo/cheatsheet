## Path Definition
```javascript
const publicDirectoryPath = path.join(__dirname, '../public')
const viewsPath = path.join(__dirname, '../templates/views')
const partialsPath = path.join(__dirname, '../templates/partials')
```

## Setup handlebars engine and views location
```javascript
app.set('view engine', 'hbs')
app.set('views', viewsPath)
hbs.registerPartials(partialsPath)
```

## Setup static directory to serve
```javascript
app.use(express.static(publicDirectoryPath))
```

## Use Express JSON
```javascript
app.use(express.json())
```

## Express serve
```javascript
app.listen(3000, () => {
  console.log('Server up on port 3000')
})
```
