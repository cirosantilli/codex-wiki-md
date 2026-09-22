<h1 id="11e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For every invertible matrix $A$,

$$
(r_C\circ f\circ l_C)(A)
=r_C((CA)^{-1})
=A^{-1}C^{-1}C
=A^{-1}=f(A).
$$

The maps $l_C$ and $r_C$ are linear. Differentiate this identity at $A=I$ and use the [chain rule](../../../../../../chain-rule.md) and part (a):

$$
r_C\bigl(Df(C)(Ch)\bigr)=-h.
$$

Thus $Df(C)(Ch)C=-h$. Given an arbitrary increment $k$, set $h=C^{-1}k$ to obtain the [derivative of matrix inversion](../../../../../../derivative-of-matrix-inversion.md)

$$
\boxed{Df(C)(k)=-C^{-1}kC^{-1}}.
$$

This also proves differentiability at every $C\in V$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
