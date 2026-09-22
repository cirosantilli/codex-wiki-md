<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

In [fixed-design nonparametric regression](../../../../../fixed-design-nonparametric-regression.md), the covariates $x_i$ are deterministic and

$$
Y_i=m(x_i)+\varepsilon_i,\qquad \mathbb E\varepsilon_i=0.
$$

For the usual finite-variance model assume independent errors with $\operatorname{Var}(\varepsilon_i)\le\sigma^2$. In [random-design nonparametric regression](../../../../../random-design-nonparametric-regression.md), the pairs $(X_i,Y_i)$ are independent observations and $m(x)=\mathbb E[Y_i\mid X_i=x]$; equivalently $Y_i=m(X_i)+\varepsilon_i$ with conditional mean-zero errors. Conditional [variances](../../../../../variance-split.md) are generally assumed bounded for risk bounds.

For a nonnegative [regression kernel](../../../../../kernel-for-nonparametric-regression.md) $K$ and a [smoothing bandwidth](../../../../../smoothing-bandwidth.md) $h>0$, the [Nadaraya–Watson estimator](../../../../../nadaraya-watson-estimator.md) is

$$
\widehat m_{\mathrm{NW}}(x)=\frac{\sum_i K((x_i-x)/h)Y_i}{\sum_iK((x_i-x)/h)},
$$

when the denominator is positive; replace $x_i$ by $X_i$ for [random-design nonparametric regression](../../../../../random-design-nonparametric-regression.md). The [local polynomial regression](../../../../../local-polynomial-regression.md) [estimator](../../../../../estimator.md) of degree $\ell$ minimizes the [weighted least squares](../../../../../weighted-least-squares.md) criterion

$$
\sum_i K(t_i)\left(Y_i-\sum_{j=0}^\ell\beta_j\frac{t_i^j}{j!}\right)^2,
\qquad t_i=\frac{x_i-x}{h},
$$

and reports $\widehat\beta_0$. If the weighted [Gram matrix](../../../../../gram-matrix.md) is invertible, this minimizer is unique. **The Nadaraya-Watson [estimator](../../../../../estimator.md) is exactly [local polynomial regression](../../../../../local-polynomial-regression.md) of degree zero.** Higher degrees reproduce nonconstant [polynomials](../../../../../polynomial-split.md) and reduce boundary [bias of an estimator](../../../../../bias-of-an-estimator.md).

The requested error bound needs **$\ell\ge s-1$ and mean-zero independent errors of uniformly bounded [variance](../../../../../variance-split.md)**, along with the matrix condition in the hint. The degree requirement is missing from the printed question. To see the problem, take $\ell=0$, $K=\mathbf1_{[-1,1]}$, $m(t)=t$, zero errors, $x=0$, and $h=n^{-1/4}$. This [regression function](../../../../../regression-function.md) has two bounded [derivatives](../../../../../derivative.md), but the local constant estimate is the average of $i/n$ for $1\le i\le N=\lfloor nh\rfloor$:

$$
\widehat m(0)-m(0)=\frac{N+1}{2n}\sim\frac h2.
$$

The scalar matrix $B=N/(nh)$ is bounded away from zero for every $n$. Nevertheless $(nh)^{-1/2}+h^2=n^{-3/8}+n^{-1/2}=o(h)$, so the printed conclusion with $s=2$ fails. A bounded-variance error hypothesis is also essential; otherwise an [expectation](../../../../../expected-value.md) bound need not even be finite.

Under the qualified hypotheses, use $U(t)=(1,t,\ldots,t^\ell/\ell!)^T$ and

$$
B_n=\frac1{nh}\sum_iU(t_i)U(t_i)^TK(t_i),\qquad
W_{ni}(x)=\frac1{nh}U(0)^TB_n^{-1}U(t_i)K(t_i).
$$

This symmetric [Gram matrix](../../../../../gram-matrix.md) has inverse [operator norm](../../../../../operator-norm.md) bounded by the reciprocal of its uniform positive eigenvalue lower bound. If $K$ is supported in $[-R,R]$, only $|x_i-x|\le Rh$ contribute. The equally spaced design and $nh\ge1$ imply that there are at most $2Rnh+1\le Cnh$ such points. The bounded kernel and bounded $U$ on this interval therefore yield

$$
\max_i|W_{ni}(x)|\le\frac C{nh},\qquad
\sum_i|W_{ni}(x)|\le C,\qquad
\sum_i W_{ni}(x)^2\le\frac C{nh}.
$$

For the stochastic part, [variance additivity for independent random variables](../../../../../variance-additivity-for-independent-random-variables.md) and [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) give

$$
\mathbb E\left|\sum_iW_{ni}(x)\varepsilon_i\right|
\le\left(\sum_iW_{ni}(x)^2\operatorname{Var}\varepsilon_i\right)^{1/2}
\le C\sigma(nh)^{-1/2}.
$$

For the deterministic part, let $Q_x$ be the [Taylor polynomial](../../../../../taylor-polynomial.md) of $m$ at $x$ of degree $s-1$. The [polynomial reproduction property of local polynomial regression](../../../../../polynomial-reproduction-property-of-local-polynomial-regression.md) gives $\sum_iW_{ni}(x)Q_x(x_i)=Q_x(x)=m(x)$. By [Taylor's theorem](../../../../../taylor-theorem.md), $|m(x_i)-Q_x(x_i)|\le C|x_i-x|^s\le Ch^s$ on the kernel window. Thus

$$
\left|\sum_iW_{ni}(x)m(x_i)-m(x)\right|
\le Ch^s\sum_i|W_{ni}(x)|\le Ch^s.
$$

Combining the two parts proves

$$
\boxed{\mathbb E|\widehat m_n(x)-m(x)|\le C\bigl((nh)^{-1/2}+h^s\bigr),\qquad \ell\ge s-1.}
$$

The argument also applies at the endpoints when the assumed matrix bound holds. With arbitrary degree, the generally valid smoothness term is $h^{\min(s,\ell+1)}$; extra symmetry can improve some interior biases but does not fix the general boundary counterexample.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
