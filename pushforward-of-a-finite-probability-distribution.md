# Pushforward of a finite probability distribution

↑ **Parent:** [Finite probability distribution](finite-probability-distribution.md)

For a [finite probability distribution](finite-probability-distribution.md) $p$ with support $S$ and a total [function](function-split.md) $f:S\to Y$, assign each image value the combined mass of its preimages. Its support is exactly the finite image $f(S)$, listed without repetitions. Every listed mass is positive because it contains at least one positive source mass.

The [fiber of a function](fiber-of-a-function.md) construction gives a [set partition](set-partition.md) of $S$, so finite summation gives $\sum_yq(y)=\sum_{x\in S}p(x)=1$. This proves nonnegativity and normalization without assuming that $f$ is injective. In code, mapping support values and then overwriting repeated image keys is incorrect; repeated keys must have their masses added. For example, mapping a uniform distribution on four consecutive [integers](integer-split.md) to parity produces two outcomes with mass one half each.

## ↑ Ancestors (7)

1. [Finite probability distribution](finite-probability-distribution.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/8/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/7/c/solution.md)
