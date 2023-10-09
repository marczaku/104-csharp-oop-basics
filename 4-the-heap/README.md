# Exercises 4 - The Heap

## Final Exercise

### Goal
```
Output:Player 1 attacks Player 2.
Output:Player 1 Damage: 0
Output:Player 2 Damage: 1
Output:Player 2 attacks Player 1.
Output:Player 1 Damage: 1
Output:Player 2 Damage: 1
Output:Player 1 attacks Player 1.
Output:Player 1 Damage: 2
Output:Player 2 Damage: 1
Output:Player 2 attacks Player 1.
Output:Player 1 Damage: 3
Output:Player 2 Damage: 1
Output:Player 3 Damage: 3
```

### Instructions
- Create a Console Project named `P4Attack`
- Define a class named `Player`
- Define a Field named `Damage` of Type `int`
- Define a Method named `Attack`
  - It takes an Argument of Type `Player` named `target`
  - When executed, it increments the Field `Damage` of the `target`
- Create a Player and assign it to Variable `player1`
- Create a Player and assign it to Variable `player2`
- Invoke `Attack` on `player1` and pass in `player2` as an argument
- Print the `Damage` Field of `player1` and `player2` to the Console
- Invoke `Attack` on `player2` and pass in `player1` as an argument
- Print the `Damage` Field of `player1` and `player2` to the Console
- Invoke `Attack` on `player1` and pass in `player1` as an argument
- Print the `Damage` Field of `player1` and `player2` to the Console
- Assign `player1` to a new Variable `player3`
- Have `player2` attack `player3`
- Print the `Damage` Field of `player1`, `player2` and `player3` to the Console

## P4_1Replacing

### Goal
```
Output:Plant is a seed.
Output:Plant is growing.
Output:Plant is a tree.
Output:Plant has already grown.
Output:Plant is a seed.
```

### Instructions
- Define a class named `Plant`
- Define a Field named `isGrown` which can store whether the Plant has grown into a tree.
- Define a Method `PrintStatus` which prints either `"Plant is a seed."` or `"Plant is a tree."` depending on its status.
- Define a Method `Grow` which prints `"Plany is growing."` and also changes the state of `isGrown`.
- Instantiate `Plant` and assign it to a variable named `plant`.
- Check the Status.
- Make it Grow.
- Check the Status.
- Make it Grow.
- Assign a new instance of class `Plant` to the same variable.
- Check the Status.