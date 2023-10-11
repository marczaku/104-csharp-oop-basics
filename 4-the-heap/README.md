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

This object teaches you that you can easily replace an object (class instance) with a new one. This will then be a completely new and fresh instance.

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

## P4_2AllTheSame

This exercise teaches you that when you assign an object (class instance), then the Reference to the same object is copied, which means that both variables point to the same target. The variables won't hold instances that just look the same, but that are the same object.

```
Output:4
Output:4
Output:4
Output:4
```

- Define a class named ScoreCounter
  - It was a Field named `Score` for counting the Score
  - It has a Method named `IncreaseScore` for increasing the Score
- Instantiate the class and assign it to Variable `one`
- Assign Variable `one` to Variable `two`
- Assign Variable `two` to Variable `three`
- Assign Variable `three` to Variable `four`
- Invoke `IncreaseScore` once on each Variable
- Print each Variable's `Score` to the Console
  - Notice that they all have the Same Score of `4` (not one!)
 
## P4_3PassingReferences

This exercise will teach you that when you pass an object to a function, the object still references the same object. It does not get cloned. This means that changes made within the function will affect the variable outside the function as well.


```
Output:This house is owned by Marc.
Output:This house is owned by Alex.
```

- Define a class named `House`
  - It has a Field named `Owner` which stores the name of the Owner
  - It has a Method named `PrintOwner` which prints `"This house is owned by XX."`
- In your `Program.cs`:
  - Add a Function named `Sell`
    - It takes an Argument of Type `House`
    - It changes the `Owner` of that `House` to `"Alex"`
  - Instantiate your `House` and assign it to a variable
  - Invoke `PrintOwner` on the Variable
  - Invoke `Sell` and pass the Variable as an Argument
  - Invoke `PrintOwner` on the Variable
