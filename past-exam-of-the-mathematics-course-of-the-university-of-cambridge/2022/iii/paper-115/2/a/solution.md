<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Give $\partial X$ the [outward-normal-first boundary orientation](../../../../../../outward-normal-first-boundary-orientation.md). The [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md) states that, for every compactly supported $(n-1)$-form $\omega$,

$$
\int_Xd\omega=\int_{\partial X}F^*\omega.
$$

Choose an oriented coordinate cover by charts into $\mathbb R^n$ or the half-space $\mathbb H^n=\{x^1\geq0\}$, and choose a [partition of unity](../../../../../../partition-of-unity.md) $(\rho_i)$ subordinate to it. Since the family is locally finite and $\omega$ has [compact support](../../../../../../compact-support.md), only finitely many $\rho_i\omega$ are nonzero. It is therefore legitimate to write both integrals as finite sums and prove the identity for a form supported in one chart.

In an interior chart the integral of an exact compactly supported top form is zero by the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md). In a boundary chart write

$$
\omega=\sum_{j=1}^n(-1)^{j-1}a_j\,dx^1\wedge\cdots\wedge\widehat{dx^j}\wedge\cdots\wedge dx^n.
$$

Integrating $d\omega=(\sum_j\partial_ja_j)dx^1\wedge\cdots\wedge dx^n$ coordinate by coordinate kills every tangential derivative. The normal derivative leaves precisely the restriction to $x^1=0$, with the sign selected by the outward-normal-first convention. This is $\int_{\partial X}F^*\omega$, proving the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
