<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $L_A$ and $R_A$ be left and right multiplication by $A$ on the [vector space](../../../../../../vector-space-split.md) $M_n(\mathbb C)$. Then $\operatorname{ad}A=L_A-R_A$. On [matrix units](../../../../../../matrix-unit.md), or from $M_n(\mathbb C)=\mathbb C^n\otimes(\mathbb C^n)^*$, one obtains

$$
\begin{aligned}\operatorname{Tr}(L_AL_B)&=n\operatorname{tr}(AB),&\operatorname{Tr}(R_AR_B)&=n\operatorname{tr}(BA),\\\operatorname{Tr}(L_AR_B)&=\operatorname{tr}A\operatorname{tr}B,&\operatorname{Tr}(R_AL_B)&=\operatorname{tr}A\operatorname{tr}B.\end{aligned}
$$

For example, the coefficient of $E_{ij}$ in $AE_{ij}B$ is $A_{ii}B_{jj}$; summing over $i,j$ proves the mixed-trace identity. Expanding the product of the two adjoint operators therefore gives the [Killing form of the general linear Lie algebra](../../../../../../killing-form-of-the-general-linear-lie-algebra.md):

$$
\operatorname{Tr}_{M_n}(\operatorname{ad}A\operatorname{ad}B)=2n\operatorname{tr}(AB)-2\operatorname{tr}A\operatorname{tr}B.
$$

For $A,B$ in the [special linear Lie algebra](../../../../../../special-linear-lie-algebra.md), both individual traces vanish. Furthermore $M_n(\mathbb C)=\mathfrak{sl}_n\oplus\mathbb CI$, and every adjoint operator kills the scalar summand, so its product has the same [trace](../../../../../../matrix-trace.md) on $M_n$ and on $\mathfrak{sl}_n$. Consequently the [Killing form of the special linear Lie algebra](../../../../../../killing-form-of-the-special-linear-lie-algebra.md) is

$$
\boxed{(A,B)_{\mathrm{ad}}=2n\operatorname{tr}(AB),\qquad\lambda=\frac1{2n}\quad(n\geq2).}
$$

No uniqueness theorem for [invariant bilinear forms on a Lie algebra](../../../../../../invariant-bilinear-form-on-a-lie-algebra.md) is needed: this calculation establishes the constant directly. For the degenerate case $n=1$, the Lie algebra is zero, both forms vanish, and proportionality does not determine a unique constant.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
