<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A collections library can supply a genuinely [generic method in Java](../../../../../../generic-method-in-java.md) whose own type parameter connects the input element and the result element type:
```
java
static <T> java.util.List<T> oneElement(T item) {
    java.util.List<T> result = new java.util.ArrayList<T>();
    result.add(item);
    return result;
}
```
For example, `List<String> xs = oneElement("sample");` is type-checked without a cast. The method can also construct a `List<Integer>` from an integer object. The standard library's `Collections.singletonList` is another example of this type relationship, though its returned list is unmodifiable.

**The benefit is one reusable implementation with compile-time argument/result consistency.** A raw `List` result would lose element-type information, invite unchecked calls and require casts that may fail later. Separate methods for every element type would duplicate code. Merely enclosing a concrete type in angle brackets, such as returning `List<String>`, does not make a method generic; the method here declares `<T>`. [Type erasure](../../../../../../type-erasure.md) means the guarantee is primarily a source-level type check, not a distinct runtime class for each type argument.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9](../../9.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
