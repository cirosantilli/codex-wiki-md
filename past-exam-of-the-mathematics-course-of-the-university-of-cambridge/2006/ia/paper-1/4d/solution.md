<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

Use these standard facts about a [power series](../../../../../power-series.md): it is absolutely convergent at every point strictly inside its [radius of convergence](../../../../../radius-of-convergence.md) and divergent at every point strictly outside it. Also, the [triangle inequality](../../../../../triangle-inequality.md) implies that a sum or difference of two absolutely convergent [series](../../../../../series-mathematics.md) is absolutely convergent.

Let $T$ be the [radius of convergence](../../../../../radius-of-convergence.md) of the coefficientwise sum. For $|z|<\min(R,S)$,

$$
\sum_{n\ge0}|(a_n+b_n)z^n|
\le\sum_{n\ge0}|a_nz^n|+\sum_{n\ge0}|b_nz^n|<\infty.
$$

Hence $T\ge\min(R,S)$.

Suppose $R<S$. If $T>R$, choose a finite $\rho$ with $R<\rho<\min(T,S)$ and choose $z$ of [complex modulus](../../../../../complex-modulus.md) $\rho$. The sum series and the $b_n$ series both converge absolutely there, so

$$
\sum_{n\ge0}|a_nz^n|
\le\sum_{n\ge0}|(a_n+b_n)z^n|+\sum_{n\ge0}|b_nz^n|<\infty,
$$

contradicting $\rho>R$. Thus $T=R$. Interchanging the series covers $S<R$, proving the [sum of power series with unequal radii of convergence](../../../../../sum-of-power-series-with-unequal-radii-of-convergence.md) rule:

$$
\boxed{T=\min(R,S).}
$$

The argument also covers a zero radius or an infinite larger radius. When the two radii are equal, cancellation can enlarge the radius, so the inequality of the radii matters.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
