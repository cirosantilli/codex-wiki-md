<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [singular value decomposition](../../../../../../singular-value-decomposition.md) $X=UDV^T$. Then

$$
(X^TX+\lambda I)^{-1}X^T
=V(D^TD+\lambda I)^{-1}D^TU^T.
$$

Each nonzero singular value $d$ contributes $d/(d^2+\lambda)\to d^{-1}$, while each zero one contributes zero. Thus

$$
\lim_{\lambda\downarrow0}\widehat\beta_\lambda
=VD^+U^TY=(X^TX)^+X^TY,
$$

using the [Moore-Penrose inverse](../../../../../../moore-penrose-inverse.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
