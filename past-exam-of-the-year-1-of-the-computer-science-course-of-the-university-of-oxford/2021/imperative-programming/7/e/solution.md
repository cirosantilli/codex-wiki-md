<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Give the two components independent [upper type bounds](../../../../../upper-type-bound.md) and immutable fields:

```
final case class BoundedPair[+A <: Base, +B <: Base](first: A, second: B)
```

Each component type must be a [subtype](../../../../../subtyping.md) of `Base`, but the two need not be the same [subtype](../../../../../subtyping.md). The pair's fields cannot be reassigned. Their read-only use permits covariant [type parameters](../../../../../type-parameter.md); the separate [upper type bounds](../../../../../upper-type-bound.md) constrain admissible instantiations.[Type Parameters and Variance Annotations: upper bounds restrict admissible arguments; immutable output positions permit covariance](../../../../../scala-2-13-basic-declarations-and-definitions-specification.md)

**The component accessors retain their precise static types.** For example, a `BoundedPair[Derived, Base]` exposes its first component as `Derived`, so derived-specific operations are available without a cast. A pair whose two fields are simply declared `Base` discards that distinction. Immutability here concerns the two stored references; it does not guarantee that the referenced [software objects](../../../../../software-object.md) have immutable internal state.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
