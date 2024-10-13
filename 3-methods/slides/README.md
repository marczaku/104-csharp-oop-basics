# Slides 3 - Methods

Methods allow you to define behaviour on classes. They are functions that each class instance has.

## Definition

You define the method similar to a function, but within the Scope `{` `}` of a `class` and using the `public`-Keyword (otherwise, you won't be able to access it in the next step):

```csharp
public class Player {
    public void SayHello() {
        Console.WriteLine("Hello");
    }
}
```

## Invocation

To invoke `class` Method you need:
- an object (class instance) reference
- to access the Member using the `.` (member-of) operator
- 
```csharp
Player first = new Player();
first.SayHello();
```

## Member Access

What makes Methods so special and why can you only invoke them on class instances? Because you can access class instance members from within the methods. That's really useful!

```csharp
public class Player {
    public int Level;
    public int Experience;
    
    public void IncreaseExperience() {
        Experience++;
        
        // Level Up
        if(Experience > 3) {
            Level++;
            Experience = 0;
        }
        
        Console.WriteLine($"Lvl: {Level}, Exp: {Experience}");
    }
}
```

```csharp
Player first = new Player();
first.IncreaseExperience(); // Lvl: 0, Exp: 1
first.IncreaseExperience(); // Lvl: 0, Exp: 2
first.IncreaseExperience(); // Lvl: 0, Exp: 3
first.IncreaseExperience(); // Lvl: 1, Exp: 0
first.IncreaseExperience(); // Lvl: 1, Exp: 1
first.IncreaseExperience(); // Lvl: 1, Exp: 2
```