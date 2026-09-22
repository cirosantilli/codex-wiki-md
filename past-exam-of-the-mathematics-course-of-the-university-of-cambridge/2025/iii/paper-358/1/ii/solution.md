<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Factor the perturbed operator on $D(A)$ as

$$
A+B=(I+BA^{-1})A.
$$

Since

$$
\|BA^{-1}\|\leq\|B\|\,\|A^{-1}\|<1,
$$

the [Neumann series](../../../../../../neumann-series.md) makes $I+BA^{-1}$ invertible. Therefore $0\notin\operatorname{Sp}(A+B)$ and

$$
(A+B)^{-1}=A^{-1}(I+BA^{-1})^{-1}.
$$

The geometric-series bound gives

$$
\boxed{
\|(A+B)^{-1}\|
\leq\frac{\|A^{-1}\|}
{1-\|B\|\,\|A^{-1}\|}}.
$$

Now choose a bounded open neighborhood $U$ of the isolated spectral component $X$ such that

$$
X\subset U\subset\{z:\operatorname{dist}(z,X)<\epsilon\},
\qquad
\partial U\subset\rho(A),
$$

and $\overline U$ meets no other component of the spectrum. Compactness of $\partial U$ gives

$$
M=\sup_{z\in\partial U}\|(A-zI)^{-1}\|<\infty.
$$

For all sufficiently large $n$, $\|B_n\|M<1$. Applying the first part to $A-zI$ shows uniformly that $\partial U\subset\rho(A+B_n)$.

The corresponding [Riesz projections](../../../../../../riesz-projection.md) are

$$
P=\frac1{2\pi i}\int_{\partial U}(zI-A)^{-1}\,dz,
\qquad
P_n=\frac1{2\pi i}\int_{\partial U}(zI-A-B_n)^{-1}\,dz.
$$

The resolvent identity and the uniform Neumann bound imply $\|P_n-P\|\to0$. The projection $P$ is nonzero because $U$ contains the nonempty spectral component $X$. Projections at distance less than one have isomorphic ranges, so $P_n\ne0$ for large $n$. Therefore $A+B_n$ has spectrum inside $U$, and any such point $z$ satisfies $\operatorname{dist}(z,X)<\epsilon$. Thus

$$
\boxed{
\inf_{z\in\operatorname{Sp}(A+B_n)}
\operatorname{dist}(z,X)<\epsilon}
$$

for every sufficiently large $n$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
