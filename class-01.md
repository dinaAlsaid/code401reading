# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-00) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-02)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

### Map

Map is an array method that loops through the array and performs a function on its items, then returns a **new** array with the **same length** of the original array.

it will take each item in the array and perform a function on it and then put it in a new array. the new array should be the same length as the original.


### Reduce

Reduce is an array method that loops through the array and performs a reducer function on its items, then returns a single value. The returned value type could be a number an array or an object.

it will take each item in the array and perform a function on it and then it will put it in a variable with a certain type and take the next item in the array and repeat. at the end there will be a resulting single value.



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

## Node and npm

### Node
Node.js is an open source server environment that works with different platforms. node.js is a JavaScript runtime ( includes everything you need to execute a program) built on Chrome’s V8 JavaScript engine.
it uses asynchronous programming.

#### how Node.js handles a file request

1. Sends the task to the computer's file system.
2. Ready to handle the next request.
3. When the file system has opened and read the file, the server returns the content to the client.

Node.js uses an event-driven, non-blocking I/O model (handle requests in parallel) that makes it lightweight and efficient.

### npm

npm is the world’s largest software registry. Open source developers from every continent use npm to share and borrow packages.

you can use it to:

* Adapt packages of code for your apps, or incorporate packages as they are.
* Download standalone tools you can use right away.
* Run packages without downloading.
* Share code with any npm user.
* Restrict code to specific developers.
* Create Orgs (organizations) to coordinate package maintenance, coding, and developers.
* Manage multiple versions of code and code dependencies.
* Update applications easily when underlying code is updated.
* Discover multiple ways to solve the same puzzle.
* Find other developers who are working on similar problems and projects.
