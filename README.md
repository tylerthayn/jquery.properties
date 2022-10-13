# jquery.properties
jQuery extension for setting data properties with listeners

## Installation

```sh
npm install @tyler.thayn/jquery.properties
```

## Usage

```js
require(['jquery', '../jquery.properties.js'], ($) => {
	$(() => {
		$('.Test').Property('MyProp', function (...args) {
			console.log(this)
			console.log(args)
		})
		$('.Test').Property('OtherProp', function (...args) {
			console.log(this)
			console.log(args)
		})
		$('.Test').Property('AnotherProp', function (...args) {
			console.log(this)
			console.log(args)
		})

		$('.Test').Property('MyProp', 'MyVal')
		$('.Test').data({OtherProp: 115, AnotherProp: true})
	})
})
```

```js
fetch('https://cdn.jsdelivr.net/npm/@tyler.thayn/jquery.properties@latest/jquery.properties.js').then(t => t.text()).then(eval)
```
