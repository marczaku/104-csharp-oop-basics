# Exercises 6 - Composition

## Final Exercise
We'll recreate a scenario where a knight in an RPG attacks another knight.

### Goal

```
Output:Knight attacks Knight with Bare Hands.
Output:Knights Shield fends off the strike.
Output:Equipping Sword...
Output:Knight attacks Knight with a Sword.
Output:Knights Shield was pierced by the Sword.
Output:Knight attacks knight with a Word.
Output:The Knight has no Shield and is wounded.
```

### Instructions
These are the rules of battle:
- If the attacker has no `Sword`, he attacks with his bare hands
    - If the defender has a `Shield`, he can fend off the strike
    - Else, he is hit
- If the attacker has a `Sword`, he attacks with it
    - If the defender has a `Shield`, he can fend off the strike, but the `Shield` is pierced and removed
    - Else, he is wounded

- Create a project named `P6GoodKnight`
- Create an `Shield` class
- Create a `Sword` class
- Create a `Knight` class.
  - With an `Shield` Field.
  - With a `Sword` Field.
  - With a `GetHit` Method with a `Sword` Parameter.
  - With an `Attack` Method with a `Knight` Parameter.
- Create two `Knight`, `attcker` and `defender`.
- Give `defender` an `Shield`
- Let `attacker` `Attack` `defender`
- Give `attacker` a `Sword`
- Let `attacker` `Attack` `defender`
- Let `attacker` `Attack` `defender`

## P6_1WellHelloThere
- Create a class named `Lightsaber`.
- Create a class named `ObiWan` with one Field named `Weapon`.
- Create an instance of the class and assign it to a variable.
- Print the variable itself to the Console.
- Print the variable's field `Lightsaber` to the Console.
- Assign a new instance of type `Lightsaber` to the variable's field `Weapon`.
- Print the variable's field `Lightsaber` to the Console.


