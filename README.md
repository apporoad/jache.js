# jache.js
jache is so easy to use for cache your any function

## key
1. your funciton must be stateless
 
## just try it
```bash
npm i --save jache.js
```

```js
const jache = require('jache.js')

function a(){
    console.log('a')
    return 'a'
}

a = jache.cache(a , {timeout : 100})

a()

var b = {
    test : (p)=>{ console.log('here is class test') ; return p},
    demo : (p)=>{  return p}
}

jache.cache(b)

console.log(b.test('hello'))
b.demo('good good day')

```

### more 
```js


```