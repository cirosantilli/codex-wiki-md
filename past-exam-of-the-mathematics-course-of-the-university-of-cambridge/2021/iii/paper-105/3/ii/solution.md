<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The preceding estimate gives constants $A,B>0$ such that, whenever $\|w\|_{H^2}\leq R$,

$$
\|\Phi(w)\|_{H^2}\leq A\|f\|_2+BR^3.
$$

Choose $R>0$ so that $BR^2\leq1/2$, and then choose $r>0$ so that $Ar\leq R/2$. If $\|f\|_2\leq r$, the closed ball $B_R(0)$ is mapped into itself.

For $w,z\in B_R(0)$, factor the [cubic gradient nonlinearity](../../../../../../cubic-gradient-nonlinearity.md) as

$$
|Dw|^2w-|Dz|^2z
=|Dw|^2(w-z)+(Dw+Dz)\mathbin\cdot D(w-z),z.
$$

The same [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) and the [Holder inequality](../../../../../../holder-inequality.md) imply

$$
\||Dw|^2w-|Dz|^2z\|_2
\leq CR^2\|w-z\|_{H^2}.
$$

The elliptic estimate therefore yields

$$
\|\Phi(w)-\Phi(z)\|_{H^2}
\leq C'R^2\|w-z\|_{H^2}.
$$

Shrinking $R$ further makes $C'R^2<1$, so $\Phi$ is a [contraction mapping](../../../../../../contraction-mapping.md) of the closed ball. This ball is complete because $H^2(U)\cap H_0^1(U)$ is a [Banach space](../../../../../../banach-space-split.md). The [contraction mapping theorem](../../../../../../contraction-mapping-theorem.md) gives a fixed point $u=\Phi(u)$, and its defining equation is

$$
-\Delta u-|Du|^2u=f,qquad u|_{\partial U}=0.
$$

**Thus the nonlinear [elliptic boundary value problem](../../../../../../elliptic-boundary-value-problem-split.md) has a solution for sufficiently small $\|f\|_2$.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
