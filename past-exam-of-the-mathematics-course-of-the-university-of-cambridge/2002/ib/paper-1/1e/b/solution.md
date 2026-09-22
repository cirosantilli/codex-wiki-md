<h1 id="1e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Yes; in fact the limit is uniformly continuous.** Given $\varepsilon>0$, [uniform convergence](../../../../../../uniform-convergence.md) provides one $N$ with $\sup_x|f_N(x)-f(x)|<\varepsilon/3$. [Uniform continuity](../../../../../../uniform-continuity.md) of this particular $f_N$ provides $\delta>0$ such that $|x-y|<\delta$ implies $|f_N(x)-f_N(y)|<\varepsilon/3$. The [triangle inequality](../../../../../../triangle-inequality.md) then gives

$$
|f(x)-f(y)|\leq|f(x)-f_N(x)|+|f_N(x)-f_N(y)|+|f_N(y)-f(y)|<\varepsilon.
$$

This same $\delta$ works at every point of $\mathbb R$, proving [uniform continuity](../../../../../../uniform-continuity.md) and therefore [continuity](../../../../../../continuous-function.md). The use of one global $N$ is exactly what fails for mere [pointwise convergence](../../../../../../pointwise-convergence.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1E](../../1e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
