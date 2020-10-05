# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-00) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-02)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

### Map

Map is an array method that loops through the array and performs a function on its items, then returns a **new** array with the **same length** of the original array.

* Syntax

```javascript
let new_array = arr.map(function callback( currentValue[, index[, array]]) {
    // return element for new_array
})
```

**Note**: The callback function should have a return value, which is the value pushed to the new array.

### Reduce

Reduce is an array method that loops through the array and performs a reducer function on its items, then returns a single value. The returned value type could be a number an array or an object.

* Syntax

```javascript
arr.reduce(callbackFunction( accumulator, currentValue, index, array) , initialValue);
```

The accumulator: is the accumulated value previously returned in the last invocation of the callbackFunction.
The currentValue: is the current element value used in the callbackFunction.
The index: is the index of the current value.
The array: is the array the reduce method is used on.
The initialValue: is the initial value used in the first invocation of the callbackFunction (it also dictates the type of the returned value).

**Note**: The initialValue, index and the array are optional.
If initialValue is not provided the index will start from 1 and the first value of the accumulator will be the first element in the array.
If initialValue is provided it will be used as the first value in the callbackFunction and the index will start from 0.

### Promises

1. Using then():

```javascript
let url2 = "https://animechanapi.xyz/api/quotes/random";
superAgent(url).then((result) => {
    console.log(result);
}
```

in this case the supreagent will send an HTTP request and create a promise then excute anything that is after (excluding what's inside the then() ). Then when the a response is recieved, the callback function inside then() is called (usually the code excuted depends on the data recieved from the response).

2. Using async/await :

```javascript
let url2 = "https://animechanapi.xyz/api/quotes/random";
(async () =>{
    try {
    let result = await superAgent(url);
    console.log(result)
    } catch {/*error handle*/}
})();
```

The async will define an asynchronous function and the await will stop the code excution (code that has the await) until the asynchronous function is completed. so in theory it does the same thing as the .then method.
notice that await doesn't work in top level code.(needs an async/ used in a function).

3. callback functions:

A callback function in itself is not asynchronous.
In general, for a function to be asynchronous when taking a callback function, it should be considered how the callback function is used in the original function.
For example the callback function in an array method can't be asynchronous since some of the current values of the callback function will depend on previous outputs.

The next example, the callback function is called asynchronously.

```javascript
function readFileAsUtf8(filename, callback)
    fs.readFile(filename, "utf8", function(err, data) =>  {
        callback(data);
    });
}
```

The callback function will be called only after the file contents have been read at some point in the future.
