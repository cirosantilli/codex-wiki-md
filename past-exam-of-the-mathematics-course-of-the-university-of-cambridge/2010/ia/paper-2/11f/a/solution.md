<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditional on $X_n=m$, the next generation is the sum of $m$ independent offspring counts, each with [probability generating function](../../../../../../probability-generating-function.md) $F_1(s)$. Hence

$$
E[s^{X_{n+1}}\mid X_n=m]=F_1(s)^m.
$$

This also holds for $m=0$, when the empty sum is zero and the empty product is one. The [law of total expectation](../../../../../../law-of-total-expectation.md) gives

$$
\boxed{F_{n+1}(s)=E[F_1(s)^{X_n}]=F_n(F_1(s)).}
$$

For complex $|s|\leq1$, the expectations are absolutely bounded because $|F_1(s)|\leq1$. This proves the [branching-process generating-function iteration](../../../../../../branching-process-generating-function-iteration.md), with $F_0(s)=s$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
