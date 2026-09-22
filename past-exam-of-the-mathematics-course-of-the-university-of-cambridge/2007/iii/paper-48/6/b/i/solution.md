<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Introduce a categorical [latent variable](../../../../../../../latent-variable.md) $Z_i$ for each observation, with $P(Z_i=j)=\alpha_j$, and let $z_{ij}=\mathbf1_{\{Z_i=j\}}$. Conditional on $Z_i=j$, $X_i$ has a [normal distribution](../../../../../../../normal-distribution.md) of mean $\mu_j$ and the shared variance $\sigma^2$. The complete-data [log-likelihood function](../../../../../../../log-likelihood.md) is

$$
\ell_c(\theta;x,z)=\sum_{i=1}^N\sum_{j=1}^kz_{ij}\log\alpha_j-\frac N2\log(2\pi\sigma^2)-\frac1{2\sigma^2}\sum_{i=1}^N\sum_{j=1}^kz_{ij}(x_i-\mu_j)^2.
$$

Initialize finite means, positive weights summing to one, and a positive common variance. At iteration $r$, the [Bayes' theorem](../../../../../../../bayes-theorem.md) gives the E-step [mixture responsibilities](../../../../../../../mixture-responsibility.md)

$$
\boxed{r_{ij}=P(Z_i=j\mid x_i,\theta^{(r)})=\frac{\alpha_j^{(r)}\exp[-(x_i-\mu_j^{(r)})^2/(2\sigma^{2(r)})]}{\sum_{\ell=1}^k\alpha_\ell^{(r)}\exp[-(x_i-\mu_\ell^{(r)})^2/(2\sigma^{2(r)})]}.}
$$

The common normal-density factor cancels. The observations' conditional labels are independent, and replacing $z_{ij}$ by their conditional expectations $r_{ij}$ gives

$$
Q(\theta\mid\theta^{(r)})=\sum_{i,j}r_{ij}\log\alpha_j-\frac N2\log\sigma^2-\frac1{2\sigma^2}\sum_{i,j}r_{ij}(x_i-\mu_j)^2+\text{constant}.
$$

Set $n_j=\sum_i r_{ij}$; because $\sum_jr_{ij}=1$, $\sum_jn_j=N$. The constrained weight maximization uses a [Lagrange multiplier](../../../../../../../lagrange-multiplier.md) $\eta$: differentiating $\sum_jn_j\log\alpha_j-\eta(\sum_j\alpha_j-1)$ gives $\alpha_j=n_j/\eta$, and summing fixes $\eta=N$. Differentiating the residual quadratic in each mean gives $\sum_i r_{ij}(x_i-\mu_j)=0$. Hence the first two M-step updates are

$$
\boxed{\alpha_j^{(r+1)}=\frac{n_j}{N},\qquad\mu_j^{(r+1)}=\frac{\sum_i r_{ij}x_i}{n_j}.}
$$

With these new means define $R=\sum_{i,j}r_{ij}(x_i-\mu_j^{(r+1)})^2$. The remaining objective in $u=\sigma^2$ is $-N\log u/2-R/(2u)$, whose derivative is $-N/(2u)+R/(2u^2)$. For $R>0$ it increases up to $u=R/N$ and decreases afterwards. Thus the shared-variance update is

$$
\boxed{\sigma^{2(r+1)}=\frac1N\sum_{i=1}^N\sum_{j=1}^kr_{ij}(x_i-\mu_j^{(r+1)})^2.}
$$

The denominator is $N$, not $N-k$ and not a separate count for each component: this is [maximum likelihood estimation](../../../../../../../maximum-likelihood-estimation.md) with one common variance. These are the [EM for Gaussian mixtures with a common variance](../../../../../../../em-for-gaussian-mixtures-with-a-common-variance.md) updates. Recompute responsibilities with the new parameters and repeat until the observed-data likelihood changes sufficiently little.

The monotonicity claim also follows directly. For positive old weights, the likelihood ratio for observation $i$ is

$$
\frac{\sum_j\alpha_j'f(x_i;\mu_j',\sigma'^2)}{\sum_j\alpha_j^{(r)}f(x_i;\mu_j^{(r)},\sigma^{2(r)})}=\sum_jr_{ij}\frac{\alpha_j'f(x_i;\mu_j',\sigma'^2)}{\alpha_j^{(r)}f(x_i;\mu_j^{(r)},\sigma^{2(r)})}.
$$

Apply the [Jensen inequality](../../../../../../../jensen-s-inequality.md) to the logarithm and sum over observations. This yields

$$
\ell(\theta')-\ell(\theta^{(r)})\geq Q(\theta'\mid\theta^{(r)})-Q(\theta^{(r)}\mid\theta^{(r)})\geq0
$$

for the maximizing M step. This proves likelihood increase, not convergence to the global maximum. Use several initializations to reduce sensitivity to local maxima. Compute responsibilities with a [log-sum-exp function](../../../../../../../log-sum-exp-function.md) normalization to avoid numerical underflow.

If $n_j=0$, that component's updated weight is zero and its mean is unidentified; retain its old mean or remove the empty component. Strictly positive interior initialization avoids this case in exact arithmetic while the variance stays positive. If $R=0$, there is no positive finite variance maximizing this M step: the objective tends to infinity as $\sigma^2\downarrow0$. Such boundary degeneracy needs a variance constraint or regularization, as discussed in the next solution. For $k=1$ the formulas reduce to the ordinary sample mean and the maximum-likelihood variance $N^{-1}\sum_i(x_i-\overline x)^2$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 48](../../../../paper-48-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
