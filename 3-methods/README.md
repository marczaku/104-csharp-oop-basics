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
