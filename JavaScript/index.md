
### theory
Js is synchronous. implemented step by step in top down manner

#### normal function
```js
function abc () {}
```

#### arrow function
```js
function abc = () => {}
```

#### callback functions
```js
function one( call_callback ) {
    console.log(" one called , calling two");
    
    call_callback();
}
function two( ){
    console.log(" two called , the end");
}

one ( two );
```
callback hell: 
callback forms relationship

![image](https://user-images.githubusercontent.com/77224604/236623983-ea1c2226-febf-4947-96e4-b784b92f3620.png)

solution for callback hell : promises
it takes instructions
![image](https://user-images.githubusercontent.com/77224604/236623989-1f8e10ef-d909-45aa-986f-f1d8dd1a1212.png)

### promise

![image](https://user-images.githubusercontent.com/77224604/236623992-d90cda5e-75ac-4c93-a665-f5549822e87e.png)
```js
let order = () => {
    return new Promise((resolve , reject) => {
        if(shop_is_open){
            resolve( 
                // call any function or write some console statement
            )
        }else{
            reject(
                // call any function or write some console statement
            )
        }
    });
};

// calling promise
order()
.then()
.then()
.then()
.catch()
.finally()
````
.finally( () => {} ) <br>
runs irrespective of promise is resolved or rejected.

#### promise chaining
.then() statements <br>
there should be no semi colons between ".then()"
#### error handling 
.catch() block <br>

### 
