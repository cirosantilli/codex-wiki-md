<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [data augmentation](../../../../../../../data-augmentation.md) labels to separate the mixture into groups. Define $n_i=\sum_j\mathbf1_{\{z_j=i\}}$, $s_i=\sum_{z_j=i}x_j$ and $Q_i(\mu_i)=\sum_{z_j=i}(x_j-\mu_i)^2$. The intended joint [posterior distribution](../../../../../../../bayesian-posterior.md) is proportional to

$$
\prod_{j=1}^n\omega_{z_j}\varphi(x_j;\mu_{z_j},v_{z_j})\prod_i\exp[-\mu_i^2/(2\tau^2)]v_i^{-\alpha-1}e^{-\beta/v_i}\omega_i^{\epsilon_i-1}.
$$

Summing over all allocation labels recovers the marginal mixture posterior. The [Gaussian mixture Gibbs updates with independent priors](../../../../../../../gaussian-mixture-gibbs-updates-with-independent-priors.md) follow by collecting the terms in each parameter.

For $\mu_i$, the conditional exponent is

$$
-\frac12\left[\left(\frac1{\tau^2}+\frac{n_i}{v_i}\right)\mu_i^2-2\frac{s_i}{v_i}\mu_i\right]+\text{constant}.
$$

Completing the square gives

$$
\boxed{\mu_i\mid\mathbf v,\boldsymbol\omega,\mathbf z,\mathbf x\sim N(m_i,V_i),\quad V_i=\left(\tau^{-2}+n_i/v_i\right)^{-1},\quad m_i=V_i s_i/v_i.}
$$

For $v_i$, the conditional density is proportional to $v_i^{-(\alpha+n_i/2)-1}\exp[-(\beta+Q_i(\mu_i)/2)/v_i]$, hence

$$
\boxed{v_i\mid\boldsymbol\mu,\boldsymbol\omega,\mathbf z,\mathbf x\sim\operatorname{InvGamma}\left(\alpha+\frac{n_i}2,\ \beta+\frac{Q_i(\mu_i)}2\right).}
$$

The independent prior on $\mu_i$ adds neither a $v_i^{-1/2}$ factor nor a $\mu_i^2/v_i$ penalty. Finally, combining the allocation counts with the [Dirichlet distribution](../../../../../../../dirichlet-distribution.md) prior gives

$$
\boxed{\boldsymbol\omega\mid\boldsymbol\mu,\mathbf v,\mathbf z,\mathbf x\sim\operatorname{Dirichlet}(\epsilon_1+n_1,\ldots,\epsilon_k+n_k).}
$$

A [Gibbs sampler](../../../../../../../gibbs-sampler.md) successively draws from these conditionals, using the most recently updated values. An empty component has $n_i=s_i=Q_i=0$, so its mean and variance conditionals reduce to their proper priors without dividing by an undefined group sample mean.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
