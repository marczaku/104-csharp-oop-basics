# Exercises 3 - Methods

## Final Exercise

### Goal
```
Output:0 Level and 0 Experience.
Input:99
Output:0 Level and 99 Experience.
Input: 5
Output: 1 Level and 4 Experience.
Input: 96
Output: 2 Level and 0 Experience.
Input: 301
Output: 5 level and 1 Experience.
```

### Instructions
- Create a Console Project named `P3LevelUp`
- Define a class named `Player`
- Define a Method named `GrantExperience`
  - It takes an argument that defines how much Experience the player is supposed to get.
  - It adds that experience to the Player's Experience.
  - Every time, the Player has 100 Experience or more, he levels up.
  - He keeps his extra experience.
  - He can theoretically level up multiple Levels at once.
- Create an instance of class `Player`
- Allow the user repeatedly to define, how much Experience he wants to grant the `Player` and use the `GrantExperience` Method to grant it.

## P3_1HelloWorld

This exercise lets you define your first Class Method.

- Create a `World` Class (in its own File `World.cs`)
- Give it a Method named `Hello`
  - It should print `"Hello, World!"` to the Console
- Invoke the Method from your `Program.cs`

## P3_2People

This exercise asks you to define a Method that reads a Value from its Field.

- Create a `Person` Class
- Give it a Field for their `Name`
- Give it a Method named `Greeting`
  - It should print `"Hello, I'm Marc!"` (or whatever their name is) to the Console
- Create an Array with 3 People
- Let the Console User decide their names
- Afterwards invoke `Greeting` on all People

## P3_3OpenDoor

This exercise asks you to define a Method that changes a class Field.

### Instructions
- Create a House Class
- It has a door that can be open or closed (`bool`)
- It has a method `OpenDoor` that opens the door
- It has a method `CloseDoor` that closes the door

- Create two houses `blueHouse` and `redHouse`
- Print for both houses whether the door is open (should be `false` and `false`)
- Open the Door at `blueHouse`
- Print for both houses whether the door is open (should be `true` and `false`)
- Open the Door at `redHouse`
- Print for both houses whether the door is open (should be `true` and `true`)
