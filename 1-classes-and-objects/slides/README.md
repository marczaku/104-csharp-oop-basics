# Slides 1 - Classes and Objects

Note: We'll use the `public` Keyword a lot in the coming chapters. It basically means that whatever you're about to define can be seen and accessed outside of the current Scope. 

## Class Definition
Classes can be defined.
```csharp
public class Player {
    
}
```

```csharp
public class Camera {

}
```

```csharp
public class Item {
    
}
```

## Types
Classes are Data Types and can be used as such:

e.g. as Variable Types:
```csharp
Player player;
```

or as Method Parameter Types:
```csharp
void Follow(Camera camera) {
}
```

or as Method Return Types:
```csharp
Item BuyItem() {
}
```

## Objects
When you use a class as a variable's Data Type, the variable can be used to store Objects, which are class instances. 

### Null
They are `null` per default, which means, they don't exist. More on this topic later in `#4 The Heap`
```csharp
Player player = default; // null
```

### Object Instantiation
They can be instantiated using the `new` Keyword:
```csharp
Item BuyItem() {
    return new Item();
}
```

```csharp
Item myFirstItem = new Item();
```

We will learn the details of this in future chapters.