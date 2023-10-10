# Exercises 2 - Fields

## Final Exercise

### Goal
You are designing a Player Class to contain all Player information of an RTS:
> It's an RTS Game in which the player can collect Gold, Stone and Wood as Resources. The player has a level and experience and can have an active or inactive VIP Subscription as well as PVP enabled or disabled. The place can configure his display name and enter his email address.

This is an example of a player:
> Player A has 200 Gold, 110 Stone, 53 Wood. He is level 12 and has 123 Experience. He has an active VIP subscription, but PVP disabled. His display name is Marc and his e-mail address marc@zaku.de

### Instructions
- Create a Console Project named `P2Fields`
- Design a Class that contain all information needed for the above player.
- Assign the information to a new instance of said class.
- Print all information of that class to the console.


## P2_1PlayerGold

### Goal
```
Output:200
```
### Instructions
- Create a Console Project named `P2_1PlayerGold`
- Create a class named `Player`
  - Add a field of type `int` named `gold`
- Define a variable of type `Player`
- Create and assign a new instance of Type `Player` to the variable
- Assign the value `200` to Field `gold` of that `Player` instance
- Print the value of Field `gold` of that `Player`  instance to the Console.

## P2_2ItemValues

### Goal
```
Output:100
Output:200
Output:300
```
### Instructions
- Create a Console Project named `P2_2ItemValues`
- Create a class named `Item`
  - Add a field of type `int` named `goldValue`
- Create an Array containing three `Items`
- Assign the value `100` to the first `Item`'s `goldValue`, `200` to the second's `goldValue` and `300` to the third's.
- Print the value of each `Item`'s `goldValue` to the Console.
