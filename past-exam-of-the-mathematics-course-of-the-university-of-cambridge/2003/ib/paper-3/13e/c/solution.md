<h1 id="13e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $h=f-g$. Choose a disc about $z_0$ contained in the [domain](../../../../../../domain-mathematical-analysis.md) $D$. Part (a) gives a convergent [Taylor series](../../../../../../taylor-series.md) there, and the accumulating [zeros](../../../../../../zero-of-a-function.md) together with part (b) force all its coefficients to vanish. Thus $h=0$ near $z_0$.

To propagate this to the entire [domain](../../../../../../domain-mathematical-analysis.md), define

$$
S=\{z\in D:h^{(n)}(z)=0\text{ for every }n\geq0\}.
$$

The set is nonempty by the preceding local argument. Each derivative is [continuous](../../../../../../continuous-function.md), so $S$ is closed relative to $D$ as the intersection of their zero sets. If $z\in S$, its [Taylor series](../../../../../../taylor-series.md) is zero on a disc about $z$, and all derivatives vanish throughout that disc; hence $S$ is open relative to $D$. [Connectedness](../../../../../../connected-space.md) forces $S=D$. Therefore **$f=g$ throughout $D$**, proving the [identity theorem for holomorphic functions](../../../../../../identity-theorem.md) rather than merely invoking it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13E](../../13e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
