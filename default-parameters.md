# ES6 Default Parameters

Funtions accept default parameters and destructuring parameters.

```js
function addToFive(addTo = 0) {
	return addTo + 5;	
}
let ex1 = addToFive();
let ex2 = addToFive(5);
console.log(ex1, ex2); // 5, 10

function fullname ({firstname, lastname}) {
	return `${firstname lastname}`;
}
const user = { firstname: 'Theodore', lastname: 'Logan', age: '20' };
let fullname = fullname(user);
console.log(`Hello ${fullname}`);
```

When destructuring you can also assign defaults.

```js
function myFunc({age = 42}) {
	console.log(age); // 42
};
myFunc({name: 'Theodor'});
```
