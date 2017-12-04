# cookie-custom
custom cookie library


## ECS5

```js
  Cookies.set('neko','my name');
  Cookies.set('usagi','my name', { expires: 5 });
  Cookies.get('neko');
  Cookies.delete('neko');
```

## with json

```js
var obj = {
  name: 'joel',
  lastname: 'gonzales'
}
```

## set json

```js
var valueJSON = JSON.stringify(obj)
Cookies.set('human', valueJSON, { expires: 5, path: '/' })
Cookies.set('human_data', valueJSON)
```

## get json

```js
var parseJSON = Cookies.get('human')
var valueParsed = JSON.parse(parseJSON)
```
