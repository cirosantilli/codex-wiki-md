<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For ordinary homoscedastic [fixed-design nonparametric regression](../../../../../fixed-design-nonparametric-regression.md), take observations $Y_i=g(x_i)+\epsilon_i$ at known distinct sites, with independent mean-zero errors of common [variance](../../../../../variance-split.md). A degree-$p$ [local polynomial estimator](../../../../../local-polynomial-regression.md) at a target $u$ solves the finite-dimensional [weighted least squares](../../../../../weighted-least-squares.md) problem

$$
\widehat\beta(u)=\operatorname*{argmin}_{\beta\in\mathbb R^{p+1}}
\sum_i K\!\left(\frac{x_i-u}{h}\right)
\left[Y_i-\sum_{r=0}^p\beta_r(x_i-u)^r\right]^2.
$$

Here $K$ is a nonnegative [regression kernel](../../../../../kernel-for-nonparametric-regression.md), $h>0$ is the [smoothing bandwidth](../../../../../smoothing-bandwidth.md), and sufficient local design rank ensures uniqueness. The estimate of the [regression function](../../../../../regression-function.md) is $\widehat g(u)=\widehat\beta_0(u)$. Each target has its own locally fitted [polynomial](../../../../../polynomial-split.md); this is not one global [polynomial](../../../../../polynomial-split.md) fit. The bandwidth controls the localization and the [bias-variance tradeoff](../../../../../bias-variance-tradeoff.md).

A [natural cubic smoothing spline](../../../../../cubic-smoothing-spline.md) instead solves the global penalized problem

$$
\widehat g_\lambda=\operatorname*{argmin}_{v\in H^2[a,b]}
\left\{\sum_i[Y_i-v(x_i)]^2+\lambda\int_a^b[v''(x)]^2\,dx\right\},\qquad\lambda>0.
$$

The [Sobolev space](../../../../../sobolev-space-split.md) here consists of functions with square-integrable weak [derivatives](../../../../../derivative.md) through order two. The minimizer is a [natural cubic spline](../../../../../natural-cubic-spline.md) with knots at the observation sites and linear tails outside the extreme sites. Equivalently one may perform the minimization on that finite-dimensional spline space: the [minimum roughness property of the natural cubic spline interpolant](../../../../../minimum-roughness-property-of-the-natural-cubic-spline-interpolant.md) shows that replacing a candidate by the natural spline with the same site values preserves the data loss and decreases the second-[derivative](../../../../../derivative.md) penalty. The [smoothing parameter](../../../../../smoothing-parameter.md) $\lambda$ controls curvature; it differs from the local bandwidth $h$.

For the interval-average observation problem, the printed upper limit in the loss is an indexing error: there are only $n-1$ responses and intervals, so a term with $i=n$ would involve the undefined $Y_n$ and $x_{n+1}$. The coherent loss uses the upper limit $n-1$. Put $\Delta_i=x_{i+1}-x_i$ and define the linear observation functionals

$$
L_iv=\frac1{\Delta_i}\int_{x_i}^{x_{i+1}}v(x)\,dx,\qquad1\leq i\leq n-1.
$$

The intended criterion on $C^1[a,b]$ is therefore

$$
S_\lambda(v)=\sum_{i=1}^{n-1}(Y_i-L_iv)^2+\lambda\int_a^b[v'(x)]^2\,dx.
$$

Unlike the ordinary [cubic smoothing spline](../../../../../cubic-smoothing-spline.md), this uses interval averages as data and a first-[derivative](../../../../../derivative.md) penalty; the resulting spline degree will be two.

Fix any candidate $v\in C^1[a,b]$. By the supplied interpolation property, there is a unique [quadratic spline](../../../../../quadratic-spline.md) $q\in C^1[a,b]$ with knots $x_1,\ldots,x_n$, constant on both exterior intervals, such that $L_iq=L_iv$ for every $i$. Put $d=v-q$. Then

$$
\int_{x_i}^{x_{i+1}}d(x)\,dx=0\qquad(1\leq i\leq n-1).
$$

On each interior knot interval $q''$ is a constant $c_i$, and on the two exterior intervals $q'=0$. Integrate $q'd'$ by parts separately on the intervals. At every knot the boundary contributions cancel because both $q'$ and $d$ are continuous; the contributions at $a$ and $b$ vanish because $q'$ is zero there. Thus

$$
\int_a^bq'(x)d'(x)\,dx
=-\sum_{i=1}^{n-1}c_i\int_{x_i}^{x_{i+1}}d(x)\,dx=0.
$$

This orthogonality is the key to the [quadratic smoothing spline for interval averages](../../../../../quadratic-smoothing-spline-for-interval-averages.md). Expanding the roughness penalty gives

$$
\int_a^b[v'(x)]^2\,dx
=\int_a^b[q'(x)]^2\,dx+\int_a^b[d'(x)]^2\,dx.
$$

The data-fit terms are equal because the interval averages are equal. Consequently,

$$
\boxed{S_\lambda(v)=S_\lambda(q)+\lambda\int_a^b[d'(x)]^2\,dx\geq S_\lambda(q).}
$$

Equality can occur only if $d'=0$ everywhere: the [derivative](../../../../../derivative.md) is continuous and its squared integral is zero. Then $d$ is constant, and any of its zero interval averages forces that constant to be zero. Therefore every minimizer must equal its matching [quadratic spline](../../../../../quadratic-spline.md) $q$.

We conclude that **the minimizer is a continuously differentiable quadratic spline with knots at the specified sites and constant tails on both exterior intervals.** Existence and uniqueness also follow from the supplied interpolation property. The interval-average map identifies the finite-dimensional space of these [quadratic splines](../../../../../quadratic-spline.md) with $\mathbb R^{n-1}$, and the criterion becomes a [strictly convex](../../../../../strictly-convex-function.md) quadratic function of that average vector: its data-fit term is $\|Y-y\|^2$, while its penalty is nonnegative and quadratic. It has a unique minimizer, and the strict equality argument above proves uniqueness in the full function class.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
