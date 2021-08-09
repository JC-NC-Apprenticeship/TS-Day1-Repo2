# Veg Scanner

Imagine you have just received your new allotment, and you're dying to get stuck in and plant some wonderful seasonal veg. Imagine all the wonderful aubergines and courgettes you could grow! The trouble is you are due to get a 3d schematic of the soil and what lies beneath and you suspect there will be tonnes of boring winter veg buried beneath the soil...

The schematic will be delivered to you in the following shape...

```js
[
    { potatoes: 12 },
    [{ onions: 3}, {}, {}, { leeks: 2 }],
    {},
    { potatoes: 2, leeks: 2 },
    { 'spring-onions': 4 }
    [{ squash: 1}, [{ onions: 3, potatoes: 1}, { potatoes: 1 }]]
]
```

Each index position will represent a section of soil grid, if it goes deeper (represented by an inner array), that array will be split into sections too. For clarity, an array within an array represents a section of soil one units depth below.

An empty section will be represented by an empty object

It won't be known how the soil is divided up. The array might be split into 4 sections (4 index positions) or it may be 8, who knows! 

You have to build a function which will handle a schematic of unknown depth and return a tally of all the known vegetables in the soil. That way you'll be able to foresee the endless months of eating leek and potato soup

## Task

Build a function which will search the schematic for veg and return them totalled up in a tally object

Examples would be:

`vegScanner([{ potatoes: 12 }]) => { potatoes: 12 }`
`vegScanner([{ potatoes: 12 }, { potatoes: 2, leeks: 2 }]) => { potatoes: 12, leeks: 2 }`
`vegScanner([{ onions: 3 }, [{}, {squash: 2}]]) => { onions: 3, squash: 2 }`

## Hints

- You won't have been given a solution to a recursive type yet, so see if you can work out a solution to this yourself.