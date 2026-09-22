<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The constructors `ZigType` and `ZagType` record which of the two alternating positions contains the last element. The tail types swap the two [type parameters](../../../../../type-parameter.md), so the return type of `lastZag` swaps them back:
```
lastZig :: Zig a b -> ZigOrZagType a b
lastZig Nil = error "lastZig: empty input"
lastZig (Cins x Nal) = ZigType x
lastZig (Cins _ zs) = lastZag zs

lastZag :: Zag a b -> ZigOrZagType b a
lastZag Nal = error "lastZag: empty input"
lastZag (Cans x Nil) = ZagType x
lastZag (Cans _ zs) = lastZig zs
```
For example, `lastZig` passes a tail of type `Zag b a` to `lastZag`, whose result then has type `ZigOrZagType a b`, exactly as required. Conversely, `lastZag` passes a `Zig b a` tail to `lastZig`. A singleton returns its element in the appropriate constructor; a longer input discards one element and uses [mutual recursion](../../../../../mutual-recursion.md) on the shorter tail. This proves correctness by [structural induction](../../../../../structural-induction.md) on the finite alternating sequence. The three source examples give **`ZigType 2`, `ZagType "D"`, and `ZigType True`**.

## ↑ Ancestors (12)

1. [B](../b.md)
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
