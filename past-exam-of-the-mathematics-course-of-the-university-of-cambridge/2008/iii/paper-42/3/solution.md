<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Iterating the recurrence yields

$$
\boxed{X_j=\rho^{j-1}Y_1+\sqrt{1-\rho^2}\sum_{k=2}^j\rho^{j-k}Y_k.}
$$

Thus every finite collection of the $X_j$ is a [linear transformation](../../../../../linear-map.md) of independent [standard normal random variables](../../../../../standard-normal-random-variable.md), and has a [multivariate Gaussian distribution](../../../../../multivariate-gaussian-distribution.md). The [expected values](../../../../../expected-value.md) are zero. Independence of the $Y_k$ gives

$$
\operatorname{Var}(X_j)=\rho^{2(j-1)}+(1-\rho^2)\sum_{l=0}^{j-2}\rho^{2l}=1.
$$

For $i<j$, the recurrence writes $X_j=\rho^{j-i}X_i$ plus a sum of future innovations independent of $X_i$. Hence $\operatorname{Cov}(X_i,X_j)=\rho^{j-i}$. The required vector law is

$$
\boxed{(X_1,\ldots,X_n)^T\sim N_n(0,R_n),\qquad (R_n)_{ij}=\rho^{|i-j|}.}
$$

The [covariance matrix](../../../../../covariance-matrix.md) is positive definite: the lower-triangular transformation from $(Y_1,\ldots,Y_n)$ has nonzero diagonal entries $1,\sqrt{1-\rho^2},\ldots,\sqrt{1-\rho^2}$. This also identifies a stationary [autoregressive process of order one](../../../../../autoregressive-process-of-order-one.md), with marginal density $f=\phi$.

With the [standard normal density](../../../../../standard-normal-density.md) as the [kernel for density estimation](../../../../../kernel-for-density-estimation.md), the two [characteristic functions](../../../../../characteristic-function.md) are $\psi(t)=e^{-t^2/2}$ and $\psi_K(ht)=e^{-h^2t^2/2}$. The [Gaussian random variable](../../../../../gaussian-random-variable.md) $X_1-X_{j+1}$ has mean zero and [variance](../../../../../variance-split.md) $2(1-\rho^j)$, so

$$
\mathbb E e^{it(X_1-X_{j+1})}=e^{-(1-\rho^j)t^2}.
$$

This expression is real. Substitution in the given integrated covariance expression, followed by the [Gaussian integral](../../../../../gaussian-integral.md) $\int_{\mathbb R}e^{-at^2}\,dt=\sqrt{\pi/a}$ for $a>0$, gives

$$
\begin{aligned}
g(j)&=\int_{\mathbb R}\left[e^{-(1+h^2-\rho^j)t^2}-e^{-(1+h^2)t^2}\right]dt\\
&=\boxed{\sqrt\pi\left[\frac1{\sqrt{1+h^2-\rho^j}}-\frac1{\sqrt{1+h^2}}\right].}
\end{aligned}
$$

To bound the total [Gaussian autoregressive kernel variance correction](../../../../../gaussian-autoregressive-kernel-variance-correction.md), apply the [mean value theorem](../../../../../mean-value-theorem.md) to $u\mapsto u^{-1/2}$. For $j\geq1$, the whole interval between $1+h^2-\rho^j$ and $1+h^2$ is bounded below by $1-\rho>0$. Therefore

$$
0\leq g(j)\leq\frac{\sqrt\pi\,\rho^j}{2(1-\rho)^{3/2}}.
$$

Summing the [geometric series](../../../../../geometric-series.md) gives the uniform bound

$$
0\leq\sum_{j=1}^{n-1}\left(1-\frac jn\right)g(j)
\leq\frac{\sqrt\pi}{2(1-\rho)^{3/2}}\frac\rho{1-\rho}.
$$

It follows from the supplied [variance](../../../../../variance-split.md) identity that

$$
\boxed{\int\operatorname{Var}(\widehat f_h(x))\,dx
=\int\operatorname{Var}(\widehat f_h^*(x))\,dx+O(n^{-1}).}
$$

The constant depends on the fixed $\rho$, but not on $h$ or $n$. In particular this applies to the requested shrinking-bandwidth regime; the covariance bound itself does not need $nh\to\infty$.

All observations have the same marginal density $f$, so dependence changes the [variance](../../../../../variance-split.md) but not the [bias of a kernel density estimator](../../../../../bias-of-a-kernel-density-estimator.md): $\mathbb E\widehat f_h=K_h*f$. Write $R(q)=\int_{\mathbb R}q^2$ and $\mu_2(K)=\int u^2K(u)\,du$. For a smooth density with $f''\in L^2$, the [integrated variance of a kernel density estimator](../../../../../integrated-variance-of-a-kernel-density-estimator.md) in the independent case is $R(K)/(nh)+O(n^{-1})$. A second-order [Taylor expansion](../../../../../taylor-expansion.md) of the [convolution](../../../../../convolution.md) gives $K_h*f-f=(h^2\mu_2(K)/2)f''+o(h^2)$ in the [L2 norm](../../../../../l2-norm.md). Thus the [bias-variance decomposition of mean squared error](../../../../../bias-variance-decomposition-of-mean-squared-error.md) gives

$$
\operatorname{MISE}(h)=\frac{R(K)}{nh}+\frac{\mu_2(K)^2R(f'')}{4}h^4+o(h^4)+O(n^{-1}).
$$

The first two terms are the [asymptotic mean integrated squared error](../../../../../asymptotic-mean-integrated-squared-error.md). The additional dependence term is smaller than $n^{-4/5}$, so the leading optimal bandwidth and optimal rate are the same as for independent data:

$$
\boxed{h_{\mathrm{AMISE}}=\left[\frac{R(K)}{n\mu_2(K)^2R(f'')}\right]^{1/5},\qquad
\operatorname{MISE}(h_{\mathrm{AMISE}})\asymp n^{-4/5}.}
$$

Here both $K$ and $f$ are the [standard normal density](../../../../../standard-normal-density.md). Since $f''(x)=(x^2-1)\phi(x)$, direct [Gaussian integrals](../../../../../gaussian-integral.md) give

$$
R(K)=\frac1{2\sqrt\pi},\qquad \mu_2(K)=1,\qquad
R(f'')=\frac1{2\pi}\int(x^2-1)^2e^{-x^2}\,dx=\frac3{8\sqrt\pi}.
$$

Consequently the explicit leading bandwidth is

$$
\boxed{h_{\mathrm{AMISE}}=\left(\frac4{3n}\right)^{1/5},\qquad
\operatorname{MISE}(h_{\mathrm{AMISE}})\sim\frac5{8\sqrt\pi}\left(\frac34\right)^{1/5}n^{-4/5}.}
$$

At this bandwidth the leading integrated [variance](../../../../../variance-split.md) is four times the leading integrated squared bias, which is also a check on the minimization constant.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
