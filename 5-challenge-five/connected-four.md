# Connected Four

## Introduction

We've all played Connect Four at least one time in our lives! See [here](https://en.wikipedia.org/wiki/Connect_Four) if you haven't for more details 😲 ...or perhaps just for a reminder.

The first to line up 4 discs is the winner

The game comes in different size variations, including 5×4, 6×5, 8×7, 9×7, 10×7, 8×8. However the standard size is 7x6 (7 columns, 6 rows).

## Task

You must come up with a function that can handle the standard grid size of 7x6, and 2 other sizes of your choosing.

The function should accept a grid and return a grid of the same size. The grid should look like the following:

```js
//7x6 grid
[
 [null,  null,  null,     null,     null,     null,     null    ],
 [null,  null,  null,     null,     null,     null,     null    ],
 [null,  null,  null,     'yellow', 'red',    null,     null    ],
 [null,  null,  'yellow', 'red',    'red',    'yellow', 'red'   ],
 [null,  null,  'red',    'yellow', 'yellow', 'yellow', 'red'   ],
 [null,  'red', 'red',    'yellow', 'yellow', 'red',    'yellow'],
]
```

Your function should accept the above grid and return a grid of the same size, but with only the winning combination of the discs showing:

```js
//7x6 grid
[
 [null,  null,  null,  null,  null,  null, null],
 [null,  null,  null,  null,  null,  null, null],
 [null,  null,  null,  null,  'red', null, null],
 [null,  null,  null,  'red', null,  null, null],
 [null,  null,  'red', null,  null,  null, null],
 [null,  'red', null,  null,  null,  null, null],
]
```

If there is no connected discs, and therefore no winner, then an empty grid should be returned from the function, like so:

```js
//7x6 grid
[
 [null, null, null, null, null, null, null],
 [null, null, null, null, null, null, null],
 [null, null, null, null, null, null, null],
 [null, null, null, null, null, null, null],
 [null, null, null, null, null, null, null],
 [null, null, null, null, null, null, null],
]
```

Your function should work like this for the standard size 7x6, and the other 2 sizes you have chosen. Of course your function should also be type safe :)