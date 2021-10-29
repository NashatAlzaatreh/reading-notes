# Node Ecosystem, TDD, CI/CD

## Array.map()

Definition and Usage

#### The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.

The map() method creates a new array with the results of calling a function for every array element.

The map() method calls the provided function once for each element in an array, in order.

map() does not execute the function for empty elements.

map() does not change the original array.

## Array.reduce()

Definition and Usage

The reduce() method executes a reducer function for each value of an array.

reduce() returns a single value which is the function's accumulated result.

reduce() does not execute the function for empty array elements.

reduce() does not change the original array.

## superagent()

```
request
   .get('/search')
   .then(res => {
      // res.body
   })
   .catch(err => {
      // err.message, err.response
   });
```

```
const ex = async (req, res) => {
const url = "https://ex.com/ee";

await axios.get(url).then((da) => {

 res.json(da);
});
};
```

## Promises

A promise is an object that may produce a single value some time in the future: either a resolved value, or a reason that it's not resolved (e.g., a network error occurred). A promise may be in one of 3 possible states: fulfilled, rejected, or pending.

## Are all callback functions considered to be Asynchronous? Why or Why Not?

Callbacks are not asynchronous by nature, but can be used for asynchronous purposes
