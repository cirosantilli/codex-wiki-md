<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $v=\mathbb E X_n^2$. For $c\geq0$, [conditional Jensen inequality](../../../../../../conditional-jensen-inequality.md) applied to the [convex function](../../../../../../convex-function.md) $x\mapsto(x+c)^2$ shows that

$$
Z_k=(X_k+c)^2
$$

is a nonnegative [submartingale](../../../../../../submartingale.md). Its integrability follows from the square integrability of $X_k$. If $X_k\geq\lambda$, then $Z_k\geq(\lambda+c)^2$, since $c\geq0$. The [Doob maximal inequality for a nonnegative submartingale](../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) yields

$$
\mathbb P\left(\max_{1\leq k\leq n}X_k\geq\lambda\right)
\leq\frac{\mathbb E(X_n+c)^2}{(\lambda+c)^2}
=\frac{v+c^2}{(\lambda+c)^2},
$$

where zero mean removes the cross term. For completeness, the maximal inequality follows by stopping at the first crossing: on the event of a crossing at $k$, the [submartingale](../../../../../../submartingale.md) property gives $\mathbb E[Z_n\mathbf1_{\{T=k\}}]\geq\mathbb E[Z_k\mathbf1_{\{T=k\}}]$. Sum over $k\leq n$, and use nonnegativity on the event of no crossing.

The derivative of the last ratio is

$$
\frac{d}{dc}\frac{v+c^2}{(\lambda+c)^2}
=\frac{2(c\lambda-v)}{(\lambda+c)^3}.
$$

For $v>0$, the minimum over $c\geq0$ is attained at $c=v/\lambda$. Substitution gives the [one-sided maximal inequality for a centered square-integrable martingale](../../../../../../one-sided-maximal-inequality-for-a-centered-square-integrable-martingale.md):

$$
\boxed{\mathbb P\left(\max_{1\leq k\leq n}X_k\geq\lambda\right)
\leq\frac{v}{\lambda^2+v}.}
$$

If $v=0$, $X_n=0$ [almost surely](../../../../../../almost-sure-convergence.md) and $X_k=\mathbb E(X_n\mid\mathcal F_k)=0$ [almost surely](../../../../../../almost-sure-convergence.md) for every $k\leq n$, so the bound also holds. The optimization is the same one underlying the [Cantelli inequality](../../../../../../cantelli-inequality.md), but the [submartingale](../../../../../../submartingale.md) argument controls the entire finite-time maximum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
