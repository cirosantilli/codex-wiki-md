<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is an [EM algorithm for a censored lognormal competing-risks mixture](../../../../../../em-algorithm-for-a-censored-lognormal-competing-risks-mixture.md). Write $Y_i=\log T_i$ and suppose $Y_i\mid I_i=j\sim N(\mu_j,\sigma_j^2)$, with mixing weights $\pi_1=\theta$, $\pi_2=1-\theta$. The missing data are $I_i$ and $Y_i$ for censored patients; neither is missing for recorded deaths or recoveries. The complete-data [log-likelihood](../../../../../../log-likelihood.md), apart from terms independent of the parameters, is

$$
\ell_c=\sum_i\sum_{j=1}^2\mathbf1_{\{I_i=j\}}\left[\log\pi_j-\log\sigma_j-\frac{(Y_i-\mu_j)^2}{2\sigma_j^2}\right].
$$

The lognormal Jacobian $-\log T_i$ is also parameter-independent and therefore does not affect the maximization.

At iteration $k$, set $z_{ij}=(\log c_i-\mu_j^{(k)})/\sigma_j^{(k)}$ for each censored patient and let $\overline\Phi(z)=1-\Phi(z)$. Bayes' rule gives the E-step class weights

$$
\boxed{w_{ij}=\frac{\pi_j^{(k)}\overline\Phi(z_{ij})}{\sum_{\ell=1}^2\pi_\ell^{(k)}\overline\Phi(z_{i\ell})}.}
$$

Given that class, $Y_i$ has a [truncated normal distribution](../../../../../../truncated-normal-distribution.md) above $\log c_i$. With the [Inverse Mills ratio](../../../../../../inverse-mills-ratio.md) $\psi(z)=\varphi(z)/\overline\Phi(z)$, compute both moments needed for the E-step:

$$
\begin{aligned}
m_{ij}&=\mu_j^{(k)}+\sigma_j^{(k)}\psi(z_{ij}),\\
v_{ij}&=(\sigma_j^{(k)})^2\left[1-\psi(z_{ij})\bigl(\psi(z_{ij})-z_{ij}\bigr)\right],\\
s_{ij}&=m_{ij}^2+v_{ij}.
\end{aligned}
$$

Thus $\mathbb E[\mathbf1_{\{I_i=j\}}\mid\text{data}]=w_{ij}$, $\mathbb E[\mathbf1_{\{I_i=j\}}Y_i\mid\text{data}]=w_{ij}m_{ij}$, and the corresponding second moment is $w_{ij}s_{ij}$. For an observed outcome $j_i$ at time $t_i$, use $w_{ij}=\mathbf1_{\{j=j_i\}}$, $m_{ij}=\log t_i$, and $s_{ij}=(\log t_i)^2$. These specify the full conditional expectation of $\ell_c$.

Put $W_j=\sum_iw_{ij}$ and let $n$ be the total number of patients. Maximizing that expected complete-data log-likelihood gives the M-step

$$
\boxed{\begin{aligned}
\theta^{(k+1)}&=W_1/n,\\
\mu_j^{(k+1)}&=\frac{\sum_iw_{ij}m_{ij}}{W_j},\\
(\sigma_j^2)^{(k+1)}&=\frac{\sum_iw_{ij}s_{ij}}{W_j}-\bigl(\mu_j^{(k+1)}\bigr)^2.
\end{aligned}}
$$

All moments on the right are evaluated at the old parameters. Repeat the E-step and M-step until the observed [log-likelihood](../../../../../../log-likelihood.md) stabilizes, using positive initial variances and mixing weights. The [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) increases that likelihood at each exact iteration, but need not find its global maximum; multiple starts help distinguish local optima. The resulting estimates give the case fatality probability $\hat\theta$ and

$$
\boxed{\widehat F(t\mid I=j)=\Phi\left(\frac{\log t-\hat\mu_j}{\hat\sigma_j}\right),\qquad t>0.}
$$

These are conditional event-time distributions, distinct from the [cumulative incidence functions](../../../../../../cumulative-incidence-function.md) $\hat\theta\widehat F(t\mid I=1)$ and $(1-\hat\theta)\widehat F(t\mid I=2)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
