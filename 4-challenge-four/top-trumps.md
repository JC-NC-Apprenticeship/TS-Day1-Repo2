# Top Trumps

You may have noticed a theme here... games from childhood ;)

If you haven't played Top Trumps at school, you clearly had something much cooler to do at break time!

## Introduction

Top Trumps is a card game of various themes (e.g. Simpsons Characters, Fast Cars, etc...) where players compete by putting down a card of their choosing and stating a category for theirs and their opponents cards to compete on. The winner of each round is the person with the highest score for that category

For more details see [here](https://en.wikipedia.org/wiki/Top_Trumps)

## Task

Create a function that will accept 2 cards, the attacker and the defender, and should return the winning card with only the categories that win

Cards should be represented as an object and should at least have a `name` and a `game` property. All other properties on the object should be categories that can be assigned a numeric score.

The function should return a card-like object with the winning categories on it

e.g.
```js
const attackersCard = {
    game: 'Northcoder Tutors',
    name: 'Alex',
    'most-zoom-calls': 180,
    beard: 5
}

const defendersCard = {
    game: 'Northcoder Tutors',
    name: 'Jim',
    'most-zoom-calls': 175
    beard: 95
}

const output = topTrumps(attackersCard, defendersCard)

/*
output:
{
    game: 'Northcoder Tutors',
    name: 'Alex',
    'most-zoom-calls': 180,
}
*/
```

If no categories are winners the return value should simply be an object with the `name` and `game` properties.

## Hint

- Think about how the inputs relate to the output, and figure out how you might create a dynamic type to match 