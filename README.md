# 1Protocol-Syntax

You define protocols in a very similar way to classes, structures, and enumerations:

```swift
protocol CustomProtocol {
    // protocol definition goes here
}
```

Custom types states that they adopt a particular protocol by placing the protocol's name after the type's name, separated by a colon, as part of their definition.

Multiple protocols can be listed, and are separated by commas:

```swift
struct CustomStructure: FirstCustomProtocol, SecondCustomProtocol {
    // structure definition goes here
}
```

If a class has a superclass, list the superclass name before any protocols it adopts, followed by a comma:

```swift
class CustomClass: CustomSuperClass, FirstCustomProtocol, SecondCustomProtocol {
    // class definition goes here
}
```