# Slides 4 - The Heap

It is important to understand how object instances work in order to use them correctly.

## The Heap

The Heap is a data structure used to keep track of all of your object instances. Every time you create an instance, the heap will:
- find enough memory for your object in its reserved RAM
- or reserve some extra RAM
- use that portion of reserved memory for your object
- and return a reference to that memory region

```csharp
public class Player {
    public int Level;
    public int Experience;
```

```csharp
Player first = new Player(); // ObjectA
Player second = new Player(); // ObjectB
```

## Passing References
Opposite to Types we've seen so far, reference types allow sharing data without copying it:
```csharp
Player first = new Player(); // ObjectA
Player second = first; // ObjectA
first.Level = 5;
Console.WriteLine(first.Level); // 5
Console.WriteLine(second.Level); // 5
```

## Garbage

Whenever you "forget" an object by losing the last reference to that class instance, you produce Garbage. The object needs to be cleaned up again, which means that the area of the Heap can be used for other objects again:

```csharp
Player first = new Player(); // ObjectA
first = new Player(); // ObjectB
```

## Garbage Collector
C# is a managed language with a Garbage Collector. The Garbage Collector is so nice and automatically cleans up after us, so we don't produce Memory Leaks. Only problem: we don't know, when exactly.
```csharp
Player first = new Player(); // ObjectA
first = new Player(); // ObjectB

// at some point down the road...
// the garbage collector will clean up ObjectA
```

## Null
Before an object has been created by a Heap, the variable points to `null`, which basically means "nothing" or "no object" or "no class instance". 