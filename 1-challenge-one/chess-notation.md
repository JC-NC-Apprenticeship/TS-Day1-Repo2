# Chess Notation Challenge

## Introduction

In Chess, there is a standard notation for recording the moves by each player.

Rows on the board are called "Ranks" and they are numbered from 1-8

columns are called "Files" and are labelled from left to right with the letters A-H

### Chess Notation Primer

#### All notation ends with the square the piece ends up on

Pawn moves can simply just have the final location

`e4` - a pawn moves to file E, and rank 4

Others are noted differently

`Nf6` - Knight moves to f6

#### Pieces are noted a capital letter

All of the pieces use their initial apart from the knight (N):

`Bh8` - bishop moves to h8
`Qb5` - queen moves to b5
`Nc3` - knight moves to c3
`Kf1` - king moves to f1
`Rb5` - rook moves to b5

#### Capturing a piece is denoted using the letter x

Pawn notation includes the file (in lower case) from the starting position:

`dxe5` - a pawn on file "d" takes a piece in position e5

All other pieces can use the following notation:

`Rxb4` - rook takes a piece on b4

See [here](<https://en.wikipedia.org/wiki/Algebraic_notation_(chess)>) for a more in depth view of how Chess notation works.

## Task

The task is to create a function that will handle the creation of this chess notation. In it's simplest form the function should implement the behaviours described in the "Chess Notation Primer" above. But you're welcome to go further and add additional functionality if you wish

As **inputs** your function should take 2 objects representing a starting square a piece moves from and a finishing square that the piece moves to.

e.g. `f({ file: 'A', rank: 2, piece: 'Q' }, { file: 'A', rank: 3, piece: null }) => 'Qa3'`

n.b Don't be concerned by the validity of each move as this would likely be done separately (in some Game logic somewhere).

The **output** from the function should be the algebraic notation to describe the move.

Output should follow the following format in described above.

## Hints

- think about creating the input types with as narrow types as possible. There are many places where there are very limited possibilities for inputs. For example there will only ever be 8 ranks in chess
