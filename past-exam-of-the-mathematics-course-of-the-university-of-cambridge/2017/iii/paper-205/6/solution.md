<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Put $\widehat\Sigma=X^TX/n$. The [Debiased Lasso](../../../../../debiased-lasso.md) correction is

$$
\boxed{\widehat b=\widehat\beta+\widehat\Theta X^T(Y-X\widehat\beta)/n.}
$$

For the [Nodewise Lasso](../../../../../nodewise-lasso.md), let $r_j=X_j-X_{-j}\widehat\gamma^{(j)}$. Its [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) are

$$
X_{-j}^Tr_j/n=\lambda_j z_j,\qquad z_j\in\partial\|\widehat\gamma^{(j)}\|_1,
$$

so $z_{jk}=\operatorname{sgn}(\widehat\gamma_k^{(j)})$ at a nonzero coefficient and $|z_{jk}|\le1$ at a zero coefficient. Multiplying by $\widehat\gamma^{(j)}$ gives the [nodewise-Lasso residual identity](../../../../../nodewise-lasso-residual-identity.md)

$$
\frac{X_j^Tr_j}{n}=\frac{\|r_j\|_2^2}{n}+\frac{(\widehat\gamma^{(j)})^TX_{-j}^Tr_j}{n}=\frac{\|r_j\|_2^2}{n}+\lambda_j\|\widehat\gamma^{(j)}\|_1=\widehat\tau_j^2.
$$

We require nonzero design columns, a necessary qualification missing from the unrestricted printed formulation. Because $\lambda_j>0$, $\widehat\tau_j^2=0$ would force both $r_j=0$ and $\widehat\gamma^{(j)}=0$, and hence $X_j=0$. Thus nonzero columns suffice for $\widehat\tau_j^2>0$ even when $p>n$ or the full [Gram matrix](../../../../../gram-matrix.md) is singular. A zero column instead gives $\widehat\tau_j^2=0$ and its coefficient is unidentifiable from $Y$; the proposed normalization and confidence interval do not exist there.

For each $j$, define $c_j\in\mathbb R^p$ by $(c_j)_j=1$ and $(c_j)_{-j}=-\widehat\gamma^{(j)}$. Set row $j$ of $\widehat\Theta$ to $c_j^T/\widehat\tau_j^2$. Since $Xc_j=r_j$,

$$
(\widehat\Theta\widehat\Sigma)_{jk}=\frac{r_j^TX_k}{n\widehat\tau_j^2},\qquad
(\widehat\Theta\widehat\Sigma)_{jj}=1,\qquad
|(\widehat\Theta\widehat\Sigma)_{jk}|\le\frac{\lambda_j}{\widehat\tau_j^2}\quad(k\ne j).
$$

This row construction is the nodewise normalization used by [van de Geer and coauthors](https://stat.ethz.ch/Manuscripts/buhlmann/AOS-desparseLasso.pdf). The [matrix](../../../../../matrix.md) $\widehat\Theta$ need not be symmetric or be an actual inverse.

Substitute the linear model into the correction. The exact decomposition is

$$
\begin{aligned}
\sqrt n(\widehat b-\beta^0)&=W+\Delta,\\
W&=\widehat\Theta X^T\varepsilon/\sqrt n,\\
\widehat\Omega&=\widehat\Theta\widehat\Sigma\widehat\Theta^T,\\
\Delta&=\sqrt n(\widehat\Theta\widehat\Sigma-I)(\beta^0-\widehat\beta).
\end{aligned}
$$

In the fixed-design [normal linear model](../../../../../normal-linear-model.md), or with $\varepsilon\mid X\sim N_n(0,\sigma^2I)$ and nodewise estimates and tuning chosen from $X$ alone, a [linear transformation](../../../../../linear-map.md) of a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) gives $W\mid X\sim N_p(0,\sigma^2\widehat\Omega)$. Marginal normality of $\varepsilon$ without this conditional assumption would not suffice for a response-dependent random design. No independence between $W$ and $\Delta$ is asserted. The diagonal cancellation and the [Holder inequality](../../../../../holder-inequality.md) give the [debiased-Lasso remainder bound](../../../../../debiased-lasso-remainder-bound.md)

$$
\boxed{\|\Delta\|_\infty\le\sqrt n\|\beta^0-\widehat\beta\|_1\max_j\frac{\lambda_j}{\widehat\tau_j^2}.}
$$

For a coordinate variance, $\widehat\Theta_jX^T=r_j^T/\widehat\tau_j^2$, whence

$$
\widehat\Omega_{jj}=\frac{\|r_j\|_2^2}{n(\widehat\tau_j^2)^2}=\frac{\widehat\tau_j^2-\lambda_j\|\widehat\gamma^{(j)}\|_1}{(\widehat\tau_j^2)^2}.
$$

Writing $z_{1-\alpha/2}$ for the corresponding [standard normal quantile](../../../../../standard-normal-quantile.md), an approximate [confidence interval](../../../../../confidence-interval.md) is

$$
\boxed{\left[\widehat b_j\ \pm\ z_{1-\alpha/2}\frac{\sigma}{\sqrt n}\frac{\sqrt{\widehat\tau_j^2-\lambda_j\|\widehat\gamma^{(j)}\|_1}}{\widehat\tau_j^2}\right].}
$$

Equivalently its half-width is $z_{1-\alpha/2}\sigma\|X_j-X_{-j}\widehat\gamma^{(j)}\|_2/(n\widehat\tau_j^2)$. We assume $0<\alpha<1$ and $\sigma>0$. For asymptotic coverage, the standardized remainder $\Delta_j/(\sigma\sqrt{\widehat\Omega_{jj}})$ must have [convergence in probability](../../../../../convergence-in-probability.md) to zero and the coordinate variance must be nondegenerate. Exact conditional normality of $W$ alone does not give finite-sample exact coverage for $\widehat b$.

One sufficient random-design regime is the [Gaussian identity design for debiased Lasso](../../../../../gaussian-identity-design-for-debiased-lasso.md): take independent rows $X_i\sim N_p(0,I_p)$, independently of $\varepsilon$, fixed $\sigma>0$, $p=p_n\to\infty$, $s=s_n\ge1$, and

$$
\log p=o(n),\qquad s\log p=o(\sqrt n).
$$

Choose $\lambda=C\sigma\sqrt{\log p/n}$ and all $\lambda_j=D\sqrt{\log p/n}$ for sufficiently large fixed $C,D$. Here is why this regime has the requested remainder bound. Uniformly over columns, their squared [norms](../../../../../norm.md) divided by $n$ tend to one, while all off-diagonal sample cross-correlations have magnitude at most a constant times $\sqrt{\log p/n}$ with [probability](../../../../../probability.md) tending to one. Taking $D$ larger makes the zero [vector](../../../../../vector.md) satisfy all nodewise [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) strictly, so $\widehat\gamma^{(j)}=0$ for every $j$ on that event, and $\widehat\tau_j^2=\|X_j\|_2^2/n\ge1/2$ eventually. This also gives $\widehat\Omega_{jj}=1/\widehat\tau_j^2\to1$ uniformly.

In this regime, the entrywise [entrywise concentration of a Gaussian Gram matrix](../../../../../entrywise-concentration-of-a-gaussian-gram-matrix.md) and [Lasso cone condition](../../../../../lasso-cone-condition.md) argument in [Gaussian identity design for debiased Lasso](../../../../../gaussian-identity-design-for-debiased-lasso.md) gives a [Compatibility condition for the Lasso](../../../../../compatibility-condition-for-the-lasso.md) bounded away from zero with [probability](../../../../../probability.md) tending to one. Together with the noise-score event and the [Basic inequality for the Lasso](../../../../../basic-inequality-for-the-lasso.md), this yields, for a fixed $C_1$,

$$
\Pr\left(\|\widehat\beta-\beta^0\|_1>C_1s\sqrt{\log p/n}\right)\longrightarrow0.
$$

For example, the cone inequality and compatibility bound give $\|\widehat\beta-\beta^0\|_1\le12\lambda s/\phi^2$ on their joint event. Therefore, with a fixed $A\ge2DC_1$,

$$
\boxed{\Pr\left(\|\Delta\|_\infty>As\log p/\sqrt n\right)\longrightarrow0.}
$$

The stated sparsity condition makes this remainder vanish and supplies the preceding confidence-interval requirement. Both dimensions may grow: $p=n^2$ and $s=\lfloor n^{1/4}\rfloor$ satisfy these assumptions. The concentration and Gaussian-design compatibility results are sufficient standard conditions here; the question does not require their proofs. The displayed rate is a high-probability fixed-constant bound, rather than only a claim of boundedness in [probability](../../../../../probability.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
