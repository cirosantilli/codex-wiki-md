<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $Z=[X,W]$. Its ridgeless minimum-norm fit is $Z^T(ZZ^T)^+Y$, so its first $p$ coordinates are

$$
\widetilde\beta_{1:p}=X^T(XX^T+WW^T)^+Y.
$$

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) applied entrywise gives $WW^T\to\lambda I_n$ almost surely as $d\to\infty$. Continuity of inversion then yields

$$
\widetilde\beta_{1:p}\longrightarrow
X^T(XX^T+\lambda I_n)^{-1}Y
=(X^TX+\lambda I_p)^{-1}X^TY=\widehat\beta_\lambda
$$

almost surely, where the middle equality is the [push-through identity](../../../../../../push-through-identity.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
