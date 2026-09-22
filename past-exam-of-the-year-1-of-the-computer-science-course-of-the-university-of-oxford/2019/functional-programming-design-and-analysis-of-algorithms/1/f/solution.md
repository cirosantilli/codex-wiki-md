<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Assign $y:u$ and $x:v$. The application `s y x` forces $s:u\to v\to w$ for a fresh type $w$; applying `f` to that result forces $f:w\to r$. No further equations identify these four type variables. The [principal type](../../../../../principal-type.md) is therefore

```
k :: (u -> v -> w) -> v -> (w -> r) -> u -> r
k s x f y = f (s y x)
```

Every compatible typing is an instance of this one, because [type inference](../../../../../type-inference.md) imposed precisely the two application constraints and no class constraints.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
