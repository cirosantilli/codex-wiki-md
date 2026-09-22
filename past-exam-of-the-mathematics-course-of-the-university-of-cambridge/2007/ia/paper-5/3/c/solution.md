<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The inference is false in both directions. Although `String` is a subtype of `Object`, [generic type invariance](../../../../../../generic-type-invariance.md) means that neither `Vector<String>` nor `Vector<Object>` is a subtype of the other. If a string vector could be used as an object vector, an arbitrary object could be inserted into storage promised to contain strings. Conversely, an object vector may already contain an `Integer`, so it cannot satisfy the contract of a string vector.

Both parameterizations are subtypes of the ordinary class `Object`, but this does not create a subtype relation between their element parameterizations. For a view accepting vectors with different element types, `Vector<?>` is appropriate; a `Vector<? extends Object>` similarly allows retrieval as `Object` without arbitrary non-null insertion. A `Vector<? super String>` accepts insertion of strings but does not promise that retrieved elements are strings. **The stated subclass relationship does not hold: mutable generic vectors are invariant.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
