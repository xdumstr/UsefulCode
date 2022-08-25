1. Run the following code in console
```js
const getMethods = (obj) => {
  let properties = new Set()
  let currentObj = obj
  do {
    Object.getOwnPropertyNames(currentObj).map(item => properties.add(item))
  } while ((currentObj = Object.getPrototypeOf(currentObj)))
  return [...properties.keys()].filter(item => typeof obj[item] === 'function')
}

```

1. Usage

```js
getMethods("")
getMethods(new String('test'))
getMethods({})
getMethods(Date.prototype)
```

[Source](https://flaviocopes.com/how-to-list-object-methods-javascript/) 
