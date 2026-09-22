<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The answer depends on the actual definitions above, especially the direction used for [duplicate removal](../../../../../duplicate-removal.md).

- `invert` works for an infinite [binary relation](../../../../../binary-relation.md) enumerated by a [lazy list](../../../../../lazy-list.md): each output needs only one input pair, and swapping preserves distinctness.
- `removedup` is productive whenever the input has infinitely many distinct values and equality tests terminate. Each next new value occurs at a finite input position and passes finitely many earlier filters. In particular, it works on the stipulated distinct-element representation of an infinite [binary relation](../../../../../binary-relation.md). On an infinite [list](../../../../../list-abstract-data-type.md) with only finitely many distinct values it emits those values but cannot certify that there is no next new value; for example, demanding the tail after the first result of `removedup (repeat 1)` diverges.
- `relcomp` does not work for arbitrary infinite inputs. Its nested [list comprehension](../../../../../list-comprehension.md) can remain forever in the inner generator. With `r = [(i,0) | i <- [0..]]` and `s = [(0,j) | j <- [0..]]`, it emits only pairs whose first component is zero, starving every later outer value. [Duplicate removal](../../../../../duplicate-removal.md) cannot repair this lack of [fair enumeration](../../../../../fair-enumeration.md).
- `transclose` does not work for a general infinite input: even its first `length s` cannot finish. It waits for finite saturation before returning any result.

Thus $\boxed{\text{inversion works; deduplication has the stated productivity condition; composition and closure fail in general}}$. A fairer enumeration may improve the latter constructions, but would be a different [algorithm](../../../../../algorithm-split.md); ordinary depth-first enumeration does not become fair through [lazy evaluation](../../../../../lazy-evaluation.md) alone.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
