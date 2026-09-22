<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Seifert surface](../../../../../../seifert-surface.md) for an [oriented knot](../../../../../../oriented-knot.md) $K$ is a compact connected oriented surface $F\subset S^3$ whose oriented boundary is $K$. For homology classes represented by oriented curves $x,y\subset F$, the [Seifert form](../../../../../../seifert-form.md) is

$$
\theta_F([x],[y])=\operatorname{lk}(x^+,y),
$$

where $x^+$ is the positive normal push-off. Choosing a basis of $H_1(F;\mathbb Z)$ gives a [Seifert matrix](../../../../../../seifert-matrix.md) $A$.

For $\omega\in S^1\setminus\{1\}$, the [Levine-Tristram signature](../../../../../../levine-tristram-signature.md) is

$$
\sigma_\omega(K)=\operatorname{sign}\bigl((1-\omega)A+(1-\overline\omega)A^T\bigr).
$$

The determinant of this Hermitian matrix vanishes away from $\omega=1$ exactly at the unit roots of the [Alexander polynomial of a knot](../../../../../../alexander-polynomial.md) $\Delta_K$. Consequently the signature is locally constant on their complement.

For $\omega=e^{i\theta}$ near $1$,

$$
(1-\omega)A+(1-\overline\omega)A^T
=i\theta(A^T-A)+O(\theta^2).
$$

The real skew-symmetric unimodular matrix $A^T-A$ has standard symplectic blocks, so the Hermitian matrix $i(A^T-A)$ has its positive and negative [eigenvalues](../../../../../../eigenvalue.md) in opposite pairs and has signature zero. Thus $\sigma_\omega(K)=0$ near $1$. If $\Delta_K$ has no unit roots, then $S^1\setminus\{1\}$ contains no singular point of the signature form and is connected, so local constancy gives $\sigma_\omega(K)=0$ everywhere. With the usual convention $\sigma_1(K)=0$, the signature vanishes identically.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
