<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Swap the components of every [ordered pair](../../../../../ordered-pair.md) using a [list comprehension](../../../../../list-comprehension.md):

```
invert :: [(a, a)] -> [(a, a)]
invert r = [(y, x) | (x, y) <- r]
```

Thus $\boxed{\operatorname{invert}(R)=R^{-1}}$, the [converse relation](../../../../../converse-relation.md). Swapping is a [bijection](../../../../../bijection.md), since doing it twice restores the original pair. Therefore distinct input pairs remain distinct; no equality constraint or [duplicate removal](../../../../../duplicate-removal.md) is necessary.

## ↑ Ancestors (12)

1. [A](../a.md)
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
