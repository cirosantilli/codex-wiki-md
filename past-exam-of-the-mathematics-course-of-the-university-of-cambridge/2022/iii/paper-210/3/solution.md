<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put

$$
r_p(u)=(1,u,\ldots,u^p)^T,
\qquad
u_i=\frac{x_i-x}{h},
\qquad
K_i=K(u_i).
$$

The degree-$p$ [local polynomial estimator](../../../../../local-polynomial-regression.md) is $\widehat m_n(x)=\widehat b_0$, where

$$
\widehat b\in\operatorname*{argmin}_{b\in\mathbb R^{p+1}}
\sum_{i=1}^n
\{Y_i-b^Tr_p(u_i)\}^2K_i.
$$

Define the [local polynomial Gram matrix](../../../../../local-polynomial-gram-matrix.md)

$$
B_{p,n}(x)=\frac1{nh}\sum_{i=1}^n
r_p(u_i)r_p(u_i)^TK_i.
$$

Assume that it is positive definite, and write

$$
\lambda_0=\lambda_{\min}\{B_{p,n}(x)\}>0.
$$

The normal equations then give

$$
\widehat m_n(x)
=\frac1n\sum_{i=1}^nw_{p,i}(x)Y_i,
\qquad
w_{p,i}(x)
=\frac1h e_1^TB_{p,n}(x)^{-1}r_p(u_i)K_i.
$$

Thus the estimator is a [linear estimator in nonparametric regression](../../../../../linear-estimator-in-nonparametric-regression.md), and the displayed $w_{p,i}$ are its [effective kernel weights](../../../../../effective-kernel-weight.md).

If $R$ is a polynomial of degree at most $p$, then $R(x+hu)=c^Tr_p(u)$ for some $c$. Feeding $Y_i=R(x_i)$ into the weighted least-squares problem gives the exact zero-residual fit $c$, whose intercept is $R(x)$. Hence the [polynomial reproduction property of local polynomial regression](../../../../../polynomial-reproduction-property-of-local-polynomial-regression.md) is

$$
\frac1n\sum_{i=1}^nw_{p,i}(x)R(x_i)=R(x).
$$

Let $\beta_0=\lceil\beta\rceil-1$. The [Hölder class](../../../../../holder-class.md) $\mathcal H(\beta,L)$ consists of functions with derivatives through order $\beta_0$ bounded by $L$ and

$$
|f^{(\beta_0)}(s)-f^{(\beta_0)}(t)|
\leq L|s-t|^{\beta-\beta_0}.
$$

The subclass $\widetilde{\mathcal H}(\beta,L)$ additionally makes every derivative of order below $\beta_0$ $L$-Lipschitz.

Suppose $p<\beta_0$. Taylor's theorem and that additional Lipschitz condition give, for the degree-$p$ Taylor polynomial $T_p$ at $x$,

$$
|m(x_i)-T_p(x_i)|
\leq\frac{L}{(p+1)!}|x_i-x|^{p+1}.
$$

On the support of $K_i$, $|u_i|\leq1$, so

$$
|w_{p,i}(x)|
\leq\frac{\sqrt{p+1}\,\|K\|_\infty}{h\lambda_0}.
$$

For the regular design $x_i=i/n$, at most $2nh+1\leq4nh$ points satisfy $|x_i-x|\leq h$ when $h\geq1/(2n)$. Polynomial reproduction cancels $T_p$, and therefore

$$
\begin{aligned}
|\operatorname{Bias}\widehat m_n(x)|
&\leq\frac1n\sum_i|w_{p,i}(x)|
|m(x_i)-T_p(x_i)|\\
&\leq
\frac{4L\sqrt{p+1}\,\|K\|_\infty}
{(p+1)!\lambda_0}h^{p+1}.
\end{aligned}
$$

**Thus the universal exponent in the question is $\gamma=1$, with the displayed choice of $C(\lambda_0,p,L,K)$.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
