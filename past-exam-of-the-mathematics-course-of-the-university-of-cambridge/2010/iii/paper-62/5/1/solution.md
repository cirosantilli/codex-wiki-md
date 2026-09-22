<h1 id="5/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the usual [spline interpolation](../../../../../../spline-interpolation.md) problem the sites are distinct and ordered; the [Schoenberg–Whitney theorem](../../../../../../schoenberg-whitney-theorem.md) then makes $A_x$ invertible under the stated support positivity. More generally, the following argument applies whenever the interpolation map in the question is well defined and $A_x$ is invertible.

Factor the [spline interpolation operator](../../../../../../spline-interpolation-operator.md) as $P_x=BA_x^{-1}R$, where

$$
Rf=(f(x_1),\ldots,f(x_n)),\qquad Bc=\sum_{j=1}^nc_jN_j.
$$

Sampling has [operator norm](../../../../../../operator-norm.md) at most one from the [supremum norm](../../../../../../supremum-norm.md) to $\ell_\infty$. Nonnegativity and the [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md) give

$$
|Bc(t)|\le\|c\|_{\ell_\infty}\sum_jN_j(t)\le\|c\|_{\ell_\infty}.
$$

Consequently $\|P_x\|\le\|A_x^{-1}\|_{\ell_\infty}$.

For the reverse bound, select a row $r$ of $A_x^{-1}$ with maximal absolute row sum, and choose $y_j=\operatorname{sgn}((A_x^{-1})_{rj})$, assigning any value of modulus at most one when the entry is zero. Then $\|y\|_{\ell_\infty}=1$ and

$$
\|A_x^{-1}y\|_{\ell_\infty}=\sum_j|(A_x^{-1})_{rj}|=\|A_x^{-1}\|_{\ell_\infty}.
$$

At distinct sites there is a continuous [piecewise linear function](../../../../../../piecewise-linear-function.md) $f$ with $f(x_j)=y_j$ and $\|f\|_\infty=1$: interpolate linearly between the ordered sites and extend constantly to the endpoints. The given [uniform-norm stability of a B-spline basis](../../../../../../uniform-norm-stability-of-a-b-spline-basis.md) therefore implies

$$
\|P_xf\|_\infty=\|BA_x^{-1}y\|_\infty\ge\frac1{d_k}\|A_x^{-1}y\|_{\ell_\infty}.
$$

Thus the [B-spline interpolation operator norm](../../../../../../b-spline-interpolation-operator-norm.md) satisfies

$$
\boxed{\frac1{d_k}\|A_x^{-1}\|_{\ell_\infty}\le\|P_x\|\le\|A_x^{-1}\|_{\ell_\infty}.}
$$

Positivity $N_i(x_i)>0$ alone, without the usual distinct-site convention, is insufficient to define an interpolation operator. For example, take order-two [B-splines](../../../../../../b-spline.md) with knots $0,1,2,3$ and $x_1=x_2=3/2$. Both diagonal values are $1/2$, but the [B-spline collocation matrix](../../../../../../b-spline-collocation-matrix.md) has identical rows $(1/2,1/2)$ and is singular. The displayed proof uses the well-defined interpolation map posited in the question; ordered distinct sites supply its standard existence guarantee.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [5](../../5.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
