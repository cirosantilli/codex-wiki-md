<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $Y=2/(1-U)$ with $U$ uniform on $(0,1)$,

$$
\Pr(Y\le y)=1-\frac2y\quad(y\ge2),\qquad q(y)=\frac2{y^2}\mathbf1_{\{y\ge2\}}.
$$

Thus $Y$ has a [Pareto distribution](../../../../../../pareto-distribution.md) and is the [importance sampling](../../../../../../importance-sampling.md) proposal, concentrated on the required tail. The target tail integrand is $f(y)=1/(\pi(1+y^2))$, so its importance weight is

$$
w(y)=\frac{f(y)}{q(y)}=\frac{y^2}{2\pi(1+y^2)}.
$$

The function returns $\widetilde\theta=n^{-1}\sum_i w(Y_i)$. Since $\mathbb E_qw(Y)=\int_2^\infty f(y)\,dy=\theta$, it is an [unbiased estimator](../../../../../../unbiased-estimator.md). For its second moment,

$$
\mathbb E_qw(Y)^2=\frac1{2\pi^2}\int_2^\infty\frac{y^2}{(1+y^2)^2}\,dy.
$$

An antiderivative is $\tfrac12(\arctan y-y/(1+y^2))$, so the integral is $\tfrac12(\pi\theta+2/5)$. Independence of the proposals gives

$$
\boxed{\operatorname{Var}(\widetilde\theta)=\frac1n\left(\frac{\theta}{4\pi}+\frac1{10\pi^2}-\theta^2\right).}
$$

This is [importance sampling of a Cauchy tail](../../../../../../importance-sampling-of-a-cauchy-tail.md), with weights between $2/(5\pi)$ and $1/(2\pi)$. Their narrow range explains the much smaller [variance](../../../../../../variance-split.md) than the indicator estimate, without appealing to nonexistent Cauchy moments.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
