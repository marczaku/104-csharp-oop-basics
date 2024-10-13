# Slides 6 - Composition

Composition describes when a Class contains other classes as members.

## Class Composition

Look at this example where a car is composited of multiple parts:

```csharp
public class Wheel {}
public class Engine {}
public class Player {}
public class Car {
    public Wheel[] Wheels;
    public Engine Engine;
    public Player Driver;
}
```

## References

Notice though, that all these Members are only referenced. Which means that classes can share the same instances as their members.

Each Bee has a Queen:
```csharp
public class Queen {}
public class Bee {
    public Queen Queen;
}
```

But all Bees can have the same Queen:
```csharp
Queen queen = new Queen();
Bee one = new Bee();
Bee two = new Bee();
Bee three = new Bee();

one.Queen = queen;
two.Queen = queen;
three.Queen = queen;
```

There might also be bees without a Queen:
```csharp
Bee one = new Bee();
one.Queen = null;
```