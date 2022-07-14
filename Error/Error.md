##  Cannot use import statement outside a module

```js
//fun.js
let fun = function(){
 console.log('hello boy')
}

export default fun;
```

```html
/*或者注了模块代码，直接script标签引入*/
<script type="moudle">
	import fun from 'fun.js'
	fun();
</script>
```

