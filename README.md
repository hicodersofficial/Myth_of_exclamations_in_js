# Myth of exclamation in JavaScript

A single exclamation in JavaScript just negates the value to "true" or the "false" and if you try add one more exclamation in front of expression than it again make validate as it was before.

```js
    const username = 'John doe'

    if(username) // This value is executed as true in if block

    // 1 exclamation negate the value which was executed as true to false.

    if(!username) // This value is executed as false

    // adding one more exclamation negate the value which was executed as false to true.
    if(!!username) // This value is executed as false
    /*
        .  if(!!!username)  false
        .  if(!!!!username)  true
        .  if(!!!!!username)  false
        .  if(!!!!!!username)  true
        .
        .
        .
        .
        . ... you can try as much you want.
    */

```
