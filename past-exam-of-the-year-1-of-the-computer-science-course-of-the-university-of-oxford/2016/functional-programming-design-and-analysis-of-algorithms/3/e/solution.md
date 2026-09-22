<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the symmetric [tree fold](../../../../../tree-fold.md) equations for the other [algebraic data type](../../../../../algebraic-data-type.md):
```
foldZag (fZag,eZag) (fZig,eZig) Nal = eZag
foldZag (fZag,eZag) (fZig,eZig) (Cans x z) =
  fZag x (foldZig (fZig,eZig) (fZag,eZag) z)
```
The most general [type signatures](../../../../../type-signature.md), using the same schematic variable names independently for each function, are
```
foldZig :: (a -> s -> r, r) -> (b -> r -> s, s)
        -> Zig a b -> r
foldZag :: (a -> s -> r, r) -> (b -> r -> s, s)
        -> Zag a b -> r
```
For `foldZig`, the first empty value has type `r`, so the first combining function must return `r`. Its label argument has type `a`. The recursively folded tail has some independent result type `s`, giving `a -> s -> r`. The second combining function consumes a `b` label and an `r` result and returns `s`, giving `b -> r -> s`. The second empty value has type `s`. Swapping the two handler pairs and the label types makes the recursive call well-typed. The identical argument applies to `foldZag`.

**The two result types need not coincide.** For example, one handler can return an [integer](../../../../../integer-split.md) and the other a [list](../../../../../list-abstract-data-type.md); forcing both results to have one type would lose [parametric polymorphism](../../../../../parametric-polymorphism.md) allowed by the definitions.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
