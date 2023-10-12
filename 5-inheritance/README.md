# Exercises 5 - Inheritance

## Final Exercise

It's up to you to design classes and their inheritance.
- Create a Project named `P5Classified`

Your Game has the following classes:
- Bread, Banana, Apple, Pear
- Sword, Axe, Pencil, Shield, Spear
- Tree, Gorilla, Chimpanzee, Sparrow, Pigeon, Hawk

Design the classes by thinking about:
- Can they be held in your hands?
- Is it an object intended to be used in Combat?
- Do they live?
- Are they known to have many Vitamins?
- Can they be eaten?

Hint: You need to add some additional classes. e.g.:
- If the given classes were `Red`, `Blue`, `Green`
- You might wanna add an additional class named `Color`

Hint: Go a bit overboard! Every time you find two or more classes that have many traits in common, give them a common parent class, e.g.:
- If the given classes were `Tulip`, `Dandelion`, `Oak`, `Fir`
- You could add `Flower` as a parent for `Tulip` and `Dandelion`
- You could add `Tree` for `Oak` and `Fir`
- and `Plant` for `Tree` and `Flower`

## P5_1Father
- Create a class named `DarthVader`
- Create a class named `Luke`
- Make `Luke` inherit from `DarthVader`

## P5_2Harvest
- Create a class named `Plant`
  - Give it a Method named `CanGrow` that prints `"I can grow."` when invoked.
- Create a class named `Grain`
  - Give it a Method named `CanBeHarvested` that prints `"I can be harvested."` when invoked.
- Create a class named `Wheat`
  - Give it a Method named `CanBeProcessedToBread` that prints `"I can be processed to bread."` when invoked.
- Make `Grain` inherit from `Plant`.
- Make `Wheat` inherit from `Grain`.
- Create instances of all three classes.
- Invoke all possible Methods on all of these classes.
