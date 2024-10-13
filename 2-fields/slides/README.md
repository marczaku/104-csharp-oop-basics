# Slides 2 - Fields

Fields allow you to define the data that your class instances will contain. It basically works like a variable that belongs to each class instance.

## Definition
You define the field similar to a variable, but within the Scope `{` `}` of a `class` and using the `public`-Keyword (otherwise, you won't be able to access it in the next step):
```csharp
public class Player {
    public int Health;
    public string Name;
}
```

In above example, every `Player` will have:
- an Integer `health` variable (Field)
- a Text `name` variable (Field)

## Assignment
To assign a value to a `class` Field you need:
- an object (class instance) reference
- to access the Member using the `.` (member-of) operator

```csharp
Player first = new Player();
first.Health = 50;
first.Name = "Marc";
```

Each `class` instance will have its own individual values:
```csharp
Player first = new Player();
Player second = new Player();
first.Name="Red";
second.Name="Blue";
```

## Access
To access a value to a `class` Field you need:
- an object (class instance) reference
- to access the Member using the `.` (member-of) operator
```csharp
Console.WriteLine(first.Health);
```

## Initialization?
Class Members are initialized to their default values automatically, there is no need to initialize them manually like with variables:

```csharp
public class Player {
    public int Health; // 0
    public bool WantsToQuit; // false (0)
    public float LevelBonus; // 0f (0)
    public char Initial; // '\0' (0)
    public string Name; // null (0)
}
```

It's valid to access these members without explicitly initializing them:

```csharp
Player first = new PLayer();
Console.WriteLine(first.Health);
```

But that's not possible with regular variables:

```csharp
int health;
Console.WriteLine(health); // ERROR
```

## Null Reference Exception

You can't access the members of "nothing":

```csharp
Player first = null;
Console.WriteLine(first.Health); // NullReferenceException
```

## Null Check

You can check, whether a value is null before accessing a Member:

```csharp
if(first != null) {
    Console.WriteLine(first.Health);
}
```

BUT ONLY DO THIS IF YOU THINK THAT IT CAN BE `null` UNDER NORMAL CONDITIONS
- e.g. if the Player sometimes carries an Item and sometimes not
- or if an NPC might have a target to walk to and sometimes not

DO NOT USE IT EVERYWHERE TO HIDE ERRORS
- i.e. do not always put `if(x != null)` every time you find a `NullReferenceException`. There might be another underlying issue that you could be hiding.
- Imagine for example, every Client (Player) is supposed to have a Character that he can move. If you just ignore if there is no movable Character (`if(playerGameObject != null){HandleInput(playerGameObject);}`), you might be hiding an underlying issue where players can't play without any error reporting.