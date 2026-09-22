<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the standard partition normalization of the [B-splines](../../../../../../b-spline.md), so $N_j\ge0$ and the [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md) gives $\sum_{j=1}^nN_j(t)\le1$. Write the interpolating [spline](../../../../../../spline-mathematics.md) as $P_xf=\sum_jc_jN_j$ and the sampled values as $y_i=f(x_i)$. The interpolation equations are $A_xc=y$, hence $c=A_x^{-1}y$ whenever the stated interpolation map is well defined. For every $t$,

$$
|P_xf(t)|\le\sum_j|c_j|N_j(t)
\le\|c\|_{\ell^\infty}\sum_jN_j(t)
\le\|c\|_{\ell^\infty}.
$$

The sampling map also satisfies $\|y\|_{\ell^\infty}\le\|f\|_\infty$. Taking [supremum norms](../../../../../../supremum-norm.md) and then the [operator norm](../../../../../../operator-norm.md) therefore proves

$$
\boxed{\|P_x\|_{L^\infty\to L^\infty}\le\|A_x^{-1}\|_{\ell^\infty\to\ell^\infty}.}
$$

This is the [B-spline interpolation operator norm](../../../../../../b-spline-interpolation-operator-norm.md) bound, and it applies on any interval containing the sampling sites on which these normalized [B-splines](../../../../../../b-spline.md) are used.

There is a small qualification to the printed hypotheses: diagonal positivity alone does not ensure uniqueness unless the usual site assumptions are supplied. For example, with two quadratic [B-splines](../../../../../../b-spline.md) on knots $1,2,3,4,5$ and $x_1=x_2=3$, both diagonal values equal $1/2$, but $A_x$ has two identical rows and is singular. The intended increasing sites $x_1<\cdots<x_n$ with $N_i(x_i)>0$ satisfy the [Schoenberg–Whitney theorem](../../../../../../schoenberg-whitney-theorem.md), making $A_x$ invertible; alternatively invertibility is implicit in the premise that $P_x$ is the unique interpolation map. The displayed bound is proved under that premise, rather than inferring invertibility from diagonal positivity alone.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
