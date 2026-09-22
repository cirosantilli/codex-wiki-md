<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

At a target $t$, [local polynomial regression](../../../../../local-polynomial-regression.md) fits a [polynomial](../../../../../polynomial-split.md) of degree at most $p$ by [weighted least squares](../../../../../weighted-least-squares.md):

$$
\widehat\beta=\arg\min_{\beta\in\mathbb R^{p+1}}\sum_{i=1}^nK\!\left(\frac{x_i-t}{h}\right)\left\{Y_i-\sum_{j=0}^p\beta_j(x_i-t)^j\right\}^2.
$$

Define the response [vector](../../../../../vector.md) $Y=(Y_1,\ldots,Y_n)^T$, the [design matrix](../../../../../design-matrix.md) $X$ by $X_{i,j+1}=(x_i-t)^j$ for $j=0,\ldots,p$, and the [diagonal matrix](../../../../../diagonal-matrix.md) $W$ by $W_{ii}=K((x_i-t)/h)$. The [normal equations for linear least squares](../../../../../normal-equations-for-linear-least-squares.md) give

$$
\boxed{\widehat\beta=(X^TWX)^{-1}X^TWY,\qquad\widehat m_h(t;p)=\widehat\beta_0.}
$$

This formula assumes the [local polynomial Gram matrix](../../../../../local-polynomial-gram-matrix.md) $X^TWX$ is invertible. It is invertible whenever at least $p+1$ distinct sites have positive weights: a nonzero degree-$p$ [polynomial](../../../../../polynomial-split.md) cannot vanish at all of them. With fixed $p$, a nonzero continuous [regression kernel](../../../../../kernel-for-nonparametric-regression.md), and $nh\to\infty$, this condition holds eventually at the target points considered here. Using weights $h^{-1}K((x_i-t)/h)$ instead gives exactly the same fit.

Use the usual unit-integral normalization $\mu_0(K)=1$. A [regression kernel](../../../../../kernel-for-nonparametric-regression.md) need not intrinsically have unit integral, but multiplying all weights by a positive constant leaves [local polynomial regression](../../../../../local-polynomial-regression.md) unchanged. With unnormalized raw moments the interior coefficient below is $\mu_2(K)/\mu_0(K)$; the version written using $\mu_2(K)$ alone requires this normalization. A zero [regression kernel](../../../../../kernel-for-nonparametric-regression.md) cannot define an estimator.

Write the local moment sums as

$$
A_r(t)=\frac1{nh}\sum_{i=1}^n(x_i-t)^rK\!\left(\frac{x_i-t}{h}\right),\qquad r=0,1,2,\ldots.
$$

The [local constant estimator](../../../../../nadaraya-watson-estimator.md) is $\widehat m_h(t;0)=\sum_iK((x_i-t)/h)Y_i/\sum_iK((x_i-t)/h)$. Since the errors have zero [mean](../../../../../expected-value.md), its [bias of an estimator](../../../../../bias-of-an-estimator.md) is the corresponding weighted average of $m(x_i)-m(t)$. By the second-order [Taylor expansion](../../../../../taylor-expansion.md), uniformly for contributing sites with $|x_i-t|\leq h$,

$$
m(x_i)-m(t)=m'(t)(x_i-t)+\frac12m''(t)(x_i-t)^2+r_{i,n},\qquad |r_{i,n}|\leq\eta_n|x_i-t|^2,
$$

where $\eta_n\to0$. This uniform remainder follows from uniform [continuity](../../../../../continuous-function.md) of $m''$ on $[0,1]$. Nonnegativity of the [regression kernel](../../../../../kernel-for-nonparametric-regression.md) therefore gives

$$
\operatorname{Bias}\{\widehat m_h(t;0)\}=m'(t)\frac{A_1(t)}{A_0(t)}+\frac12m''(t)\frac{A_2(t)}{A_0(t)}+o(h^2)
$$

whenever $A_0$ tends to a positive limit and $A_2=O(h^2)$.

For fixed interior $x$, the moment approximations give $A_0(x)=1+o(1)$, $A_1(x)=O(n^{-1})$, and $A_2(x)=h^2\mu_2(K)+o(h^2)$. The hypothesis $nh^2\to\infty$ makes $n^{-1}=o(h^2)$, so the odd-moment contribution is negligible at second order. Thus

$$
\boxed{\mathbb E\widehat m_h(x;0)-m(x)=\frac12h^2\mu_2(K)m''(x)+o(h^2).}
$$

The symmetry of the [regression kernel](../../../../../kernel-for-nonparametric-regression.md) is what removes the first-order interior [bias of an estimator](../../../../../bias-of-an-estimator.md).

At $z_n=\alpha h$, the rescaled observation window is truncated to $[-\alpha,1]$. Put $\mu_{r,\alpha}=\int_{-\alpha}^1u^rK(u)\,du$ and $\beta_r=\mu_{r,\alpha}/\mu_{0,\alpha}$. Symmetry, nonnegativity, and unit mass give $\mu_{0,\alpha}\geq1/2$. The supplied moment approximations already imply the leading [boundary bias of local constant regression](../../../../../boundary-bias-of-local-constant-regression.md):

$$
\mathbb E\widehat m_h(z_n;0)-m(z_n)=h\beta_1m'(0)+o(h).
$$

To retain the second-order term rigorously, we need slightly more precise control of the first moment. The rescaled grid $u_i=i/(nh)-\alpha$ has spacing $1/(nh)$. Each truncated function $u^rK(u)\mathbf1_{[-\alpha,1]}$ has [bounded variation](../../../../../total-variation-of-a-function.md), because $K$ is continuously differentiable on its support. The [Riemann sum](../../../../../riemann-sum.md) error is bounded by this variation times the grid spacing: summing the oscillation bounds on the grid cells proves

$$
\frac{A_r(z_n)}{h^r}=\mu_{r,\alpha}+O((nh)^{-1}).
$$

Endpoint cells, including the omitted site at zero, contribute the same error order. Consequently

$$
\frac{A_1(z_n)}{A_0(z_n)}=h\beta_1+O(n^{-1}),\qquad
\frac{A_2(z_n)}{A_0(z_n)}=h^2\beta_2+O(h/n).
$$

Both discretization errors are $o(h^2)$ under $nh^2\to\infty$. The preceding [Taylor expansion](../../../../../taylor-expansion.md) therefore proves the [second-order boundary expansion for local constant regression](../../../../../second-order-boundary-expansion-for-local-constant-regression.md):

$$
\boxed{\mathbb E\widehat m_h(z_n;0)-m(z_n)=h\beta_1m'(z_n)+\frac12h^2\beta_2m''(z_n)+o(h^2).}
$$

Equivalently, expanding the [derivatives](../../../../../derivative.md) about zero gives

$$
\boxed{\mathbb E\widehat m_h(z_n;0)-m(z_n)=h\beta_1m'(0)+h^2\left(\alpha\beta_1+\frac12\beta_2\right)m''(0)+o(h^2).}
$$

In general the truncated first moment is nonzero, so the boundary [bias of an estimator](../../../../../bias-of-an-estimator.md) has order $h$, although it can be smaller when $m'(0)=0$ or the omitted part of the [regression kernel](../../../../../kernel-for-nonparametric-regression.md) carries no mass.

For [local linear regression](../../../../../local-linear-regression.md), the [polynomial reproduction property of local polynomial regression](../../../../../polynomial-reproduction-property-of-local-polynomial-regression.md) removes the constant and linear terms exactly. Let $\Delta=A_0A_2-A_1^2$. Its [effective kernel weights](../../../../../effective-kernel-weight.md) are

$$
l_i(t)=\frac{K((x_i-t)/h)}{nh}\frac{A_2-A_1(x_i-t)}{\Delta},
$$

so $\sum_i l_i=1$, $\sum_i l_i(x_i-t)=0$, and

$$
\sum_i l_i(x_i-t)^2=\frac{A_2^2-A_1A_3}{\Delta}.
$$

At either an interior or the specified boundary target, $\Delta$ is asymptotic to a positive constant times $h^2$. At the boundary that constant is $\mu_{0,\alpha}\mu_{2,\alpha}-\mu_{1,\alpha}^2>0$, the mass squared times the [variance](../../../../../variance-split.md) of the continuous normalized truncated [regression kernel](../../../../../kernel-for-nonparametric-regression.md). Moreover $\sum_i|l_i|=O(1)$, as follows by bounding $|A_2-A_1(x_i-t)|=O(h^2)$ in the window. Thus the [Taylor remainder](../../../../../taylor-remainder.md) still contributes $o(h^2)$, even though some [effective kernel weights](../../../../../effective-kernel-weight.md) may be negative. In particular,

$$
\operatorname{Bias}\{\widehat m_h(z_n;1)\}=\frac12h^2m''(0)\frac{\mu_{2,\alpha}^2-\mu_{1,\alpha}\mu_{3,\alpha}}{\mu_{0,\alpha}\mu_{2,\alpha}-\mu_{1,\alpha}^2}+o(h^2).
$$

At an interior point this coefficient reduces to $\mu_2(K)$ by symmetry and normalization. Hence **local linear regression has bias $O(h^2)$ at both interior and boundary points**; its linear reproduction removes the generic order-$h$ boundary term.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
