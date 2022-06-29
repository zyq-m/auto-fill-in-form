# Auto-Fill-In-Form

This script work for **radio button input only**. It automate to fill in form.

Fixed:

```js
const input = document.querySelectorAll("input");

const arrInput = Array.from(input)
  .filter(input => input.value == 5)
  .map(input => (input.checked = true));
```

Random:

```js
const input = document.querySelectorAll("input");

const random = () => {
  return Math.floor(Math.random() * 5 + 1);
};

const arrInput = Array.from(input)
  .filter(input => input.value == random())
  .map(input => (input.checked = true));
```

Customize:

Just change the value as desire. For example:

```js
const input = document.querySelectorAll("input");

const arrInput = Array.from(input)
  .filter(input => input.value == 3)
  .map(input => (input.checked = true));
  
// input.value has been changed to 3
```

## How to use?

You are recommended to use laptop/desktop to perform this action.

1. Copy the code, either fixed or random
2. Right click on the form site and choose 'Inspect'
3. Try to find 'Console' option beside the 'Element'
4. Paste the code you copied and hit 'Enter'
