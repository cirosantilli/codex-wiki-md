<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $r=k-1$. The linear-reproduction request requires $k\ge2$, which we use for that final step. Since $\psi_i=\omega_i/r!$, the useful [normalized Marsden dual functional](../../../../../normalized-marsden-dual-functional.md) is

$$
\boxed{\lambda_i(p)=\sum_{j=0}^{r}(-1)^j p^{(j)}(x)\,
\psi_i^{(r-j)}(x)}.
$$

There is no further factor $1/r!$ outside this sum: it has already been included in $\psi_i$.

To derive the formula directly from [Marsden's identity](../../../../../marsden-identity.md), [Taylor's theorem](../../../../../taylor-theorem.md) for the [polynomial](../../../../../polynomial-split.md) $p$ around the arbitrary point $x$ gives

$$
p(t)=\sum_{j=0}^r\frac{(-1)^j}{j!}p^{(j)}(x)(x-t)^j.
$$

On the other hand,

$$
\partial_x^{\,r-j}(x-t)^r=\frac{r!}{j!}(x-t)^j.
$$

Differentiate [Marsden's identity](../../../../../marsden-identity.md) $r-j$ times in $x$, multiply by $(-1)^jp^{(j)}(x)/r!$, and sum over $j$. The left side becomes $p(t)$, while the right side becomes

$$
\boxed{p(t)=\sum_{i=1}^n\lambda_i(p)N_i(t)},\qquad t\in[t_k,t_{n+1}].
$$

Only finite sums and derivatives of [polynomials](../../../../../polynomial-split.md) are involved.

Independence of the auxiliary point does not require an assumption about uniqueness of an expansion. Differentiate the formula for $\lambda_i$ itself:

$$
\lambda_i'(x)=\sum_{j=0}^r(-1)^j
\left[p^{(j+1)}(x)\psi_i^{(r-j)}(x)
+p^{(j)}(x)\psi_i^{(r-j+1)}(x)\right]=0.
$$

The first summand at $j=r$ and the second at $j=0$ vanish because both [polynomials](../../../../../polynomial-split.md) have degree at most $r$. All remaining terms cancel after shifting the index by one. Therefore $\lambda_i(p)$ is a constant in $x$, and it is visibly a [linear functional](../../../../../linear-functional.md) of $p$.

For $p(t)=a+bt$, only $j=0,1$ remain. The leading two coefficients of the monic knot [polynomial](../../../../../polynomial-split.md) give

$$
\psi_i^{(r)}(x)=1,\qquad
\psi_i^{(r-1)}(x)=x-\frac1r\sum_{\ell=1}^r t_{i+\ell}
=x-t_i^*.
$$

It follows that

$$
\lambda_i(p)=a+bx-b(x-t_i^*)=a+bt_i^*=p(t_i^*).
$$

Substituting into the expansion proves

$$
\boxed{p(t)=\sum_{i=1}^n p(t_i^*)N_i(t)}
$$

on the basic knot interval. Thus the [Greville abscissae](../../../../../greville-abscissa.md) are exactly the sampling coefficients that reproduce linear [polynomials](../../../../../polynomial-split.md); the constant case also gives the [subpartition of unity for B-splines](../../../../../subpartition-of-unity-for-b-splines.md) with equality on this interval.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
