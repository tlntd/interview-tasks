## Object Oriented Programming Tasks

You can use language of your choice to solve these tasks, but solve the 
problems using Object Oriented approach. Try to use best programming practices 
when writing solutions. Focus more on code readability and coding 
conventions, not trying to create the most efficient and compact 
solution (which are often really hard to read/understand).

### Problem 1

Write a class Block that creates a block. The constructor should take an array as an argument, 
this will contain 3 integers of the form [width, length, height] from which the Block 
should be created.

Define these methods:

```
`getWidth()` return the width of the `Block`
`getLength()` return the length of the `Block`
`getHeight()` return the height of the `Block`
`getVolume()` return the volume of the `Block`
`getSurfaceArea()` return the surface area of the `Block`
```

For Example:
```
Block b = new Block(new int[]{2,4,6})
  
b.getWidth() // -> 2
b.getLength() // -> 4
b.getHeight() // -> 6
b.getVolume() // -> 48
b.getSurfaceArea() // -> 88
```

### Problem 2

Automate bingo card creation by creating an object with a method:

```
BingoCard.getCard()
```

A Bingo card contains 24 unique and random numbers according to this scheme:
- 5 numbers from the B column in the range 1 to 15
- 5 numbers from the I column in the range 16 to 30
- 4 numbers from the N column in the range 31 to 45
- 5 numbers from the G column in the range 46 to 60
- 5 numbers from the O column in the range 61 to 75

The card must be returned as an array of Bingo style numbers:

```
{ "B14", "B12", "B5", "B6", "B3", "I28", "I27", ... }
```

The numbers must be in the order of their column: B, I, N, G, O. Within the columns the order of the numbers is random.

![bingo-card](https://s-media-cache-ak0.pinimg.com/736x/6a/a2/e4/6aa2e44f7a3e9749655a9d60c6354fbd.jpg)
