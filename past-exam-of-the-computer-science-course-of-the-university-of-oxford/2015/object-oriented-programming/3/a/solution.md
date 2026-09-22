<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For primitive values, [Java](../../../../../java-programming-language.md) `==` compares values, subject to the primitive type's rules. For references, `==` compares [object identity](../../../../../object-identity.md): it asks whether the references designate the same [software object](../../../../../software-object.md), or are both null. The `equals(Object)` [object method](../../../../../object-method.md) permits a [software class](../../../../../class-programming.md) to define [value equality](../../../../../value-equality.md). Its inherited `Object` implementation still uses [object identity](../../../../../object-identity.md), so meaningful content comparison requires an appropriate override.[equals(Object), default identity semantics and the equality contract](../../../../../java-8-object-api-documentation.md)

For example:

```
String a = new String("wall");
String b = new String("wall");
boolean sameObject = (a == b);  // false
boolean sameText = a.equals(b); // true
```

The two allocations have different [object identities](../../../../../object-identity.md) but equal text. Using separately allocated [String data type](../../../../../string-data-type.md) values avoids relying on literal interning. A `null` receiver cannot receive an `equals` call; `java.util.Objects.equals(a,b)` is a null-safe comparison. An `equals` implementation should define an [equivalence relation](../../../../../equivalence-relation.md) and equal [software objects](../../../../../software-object.md) must have equal `hashCode()` results.[equals(Object) and hashCode() contracts](../../../../../java-8-object-api-documentation.md) The distinction is

$$
\boxed{\text{reference }\texttt{==}:\text{ identity};\qquad\texttt{equals}:\text{ the class's declared equality}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Object oriented programming](../../../object-oriented-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
