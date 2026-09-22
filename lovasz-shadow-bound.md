<h1 id="lovasz-shadow-bound">Lovász shadow bound</h1>

↑ **Parent:** [Kruskal-Katona theorem](kruskal-katona-theorem.md)

For a nonempty $r$-[uniform set family](uniform-set-family.md), define $x>r-1$ by $|\mathcal F|=\binom xr$ using real [binomial coefficients](binomial-coefficient.md). Then its [lower shadow](lower-shadow.md) has at least $\binom{x}{r-1}$ members. This continuous estimate is often easier to use than the exact integer expansion in the [Kruskal-Katona theorem](kruskal-katona-theorem.md).

A short proof uses [coordinate shifts of a set family](coordinate-shifts-of-a-set-family.md). In a fully left-shifted [set family](set-family.md) split at coordinate one into $\mathcal F_0$ and $\mathcal F_1$, deleting one in the present section. The shifting property implies $\partial\mathcal F_0\subseteq\mathcal F_1$, and the total [lower shadow](lower-shadow.md) has size $|\mathcal F_1|+|\partial\mathcal F_1|$. Induct on uniformity and, at fixed uniformity, on [set family](set-family.md) size. If $|\mathcal F_1|<\binom{x-1}{r-1}$, the [Pascal's identity](pascal-s-rule.md) and the size [mathematical induction](mathematical-induction.md) force $|\partial\mathcal F_0|>\binom{x-1}{r-1}$, a contradiction. The uniformity [mathematical induction](mathematical-induction.md) applied to $\mathcal F_1$, followed by the [Pascal's identity](pascal-s-rule.md), proves the estimate. Integer $x$ is sharp for the full $r$-level on $x$ coordinates.

## ↑ Ancestors (8)

1. [Kruskal-Katona theorem](kruskal-katona-theorem.md)
2. [Lower shadow](lower-shadow.md)
3. [Set family shadow](set-family-shadow.md)
4. [Extremal set theory](extremal-set-theory-split.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Effective ground-set parameter of a hereditary uniform layer](effective-ground-set-parameter-of-a-hereditary-uniform-layer.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-11/1/solution.md)
