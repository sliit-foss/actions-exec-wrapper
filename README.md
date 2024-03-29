# actions-exec-wrapper

A wrapper around the [@actions/exec](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiZ6tHV0Mr4AhXhTGwGHUPnBJ0QFnoECAoQAQ&url=https%3A%2F%2Fwww.npmjs.com%2Fpackage%2F%40actions%2Fexec&usg=AOvVaw26dWB7pmcPpZtcQ8teo8Qe) module which promisifies the console output of a command

---

## Installation

```js
# using npm
npm install actions-exec-wrapper

# using yarn
yarn add actions-exec-wrapper
```
## Usage

```js
# using require
const exec = require("actions-exec-wrapper").default;

# using import
import exec from "actions-exec-wrapper";
```

## Example<br/>

```js
exec('npm --version').then(result => {
  console.log(result);
}).catch(error => {
  console.log(error);
})
```
