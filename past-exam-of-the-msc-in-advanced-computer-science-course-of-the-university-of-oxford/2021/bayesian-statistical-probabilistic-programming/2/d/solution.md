<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The two limiting-case names in the printed bullets are reversed.** Fully reparameterized continuous choices give a [reparameterization gradient](../../../../../reparameterization-gradient.md); non-reparameterized discrete choices give a [score-function gradient estimator](../../../../../score-function-gradient-estimator.md). Here are both reductions, including the extra term that vanishes only after taking an [expectation](../../../../../expected-value-split.md).

When all choices are reparameterized with parameter-independent base noise, $s_\lambda=s$ and $\nabla_\lambda\log s=0$. The expression in part (c) becomes

$$
\nabla_\lambda\mathcal L=\mathbb E_s\left[\nabla_\lambda\{\log p(t_\lambda(\varepsilon),x)-\log q_\lambda(t_\lambda(\varepsilon))\}\right].
$$

Differentiating along the sampled transformation is precisely the [pathwise gradient](../../../../../reparameterization-gradient.md), also called the [reparameterization gradient](../../../../../reparameterization-gradient.md). There is no [score function](../../../../../informant-function.md) of the parameter-independent base law.

When all choices are discrete and left untransformed, $t_\lambda(\varepsilon)=\varepsilon=z$ and $s_\lambda=q_\lambda$. Set $S_\lambda(z)=\nabla_\lambda\log q_\lambda(z)$ and $W_\lambda(z,x)=\log p(z,x)-\log q_\lambda(z)$. Since $p$ has no variational parameter, the integrand in part (c) is

$$
S_\lambda(z)W_\lambda(z,x)-S_\lambda(z)=S_\lambda(z)(W_\lambda(z,x)-1).
$$

[Normalization](../../../../../normalization.md) gives the zero-mean [score function](../../../../../informant-function.md) identity

$$
\mathbb E_{q_\lambda}S_\lambda=\sum_z\nabla_\lambda q_\lambda(z)=\nabla_\lambda1=0.
$$

Thus

$$
\boxed{\nabla_\lambda\mathcal L=\mathbb E_{q_\lambda}[S_\lambda W_\lambda]=\mathbb E_{q_\lambda}[S_\lambda(W_\lambda-1)].}
$$

The first expression is the usual [score-function gradient estimator](../../../../../score-function-gradient-estimator.md); the second has a [constant score baseline](../../../../../constant-score-baseline.md) of one. The two random integrands are generally different even though their [expectations](../../../../../expected-value-split.md) agree. A suitable [constant score baseline](../../../../../constant-score-baseline.md) can reduce [variance](../../../../../variance-split.md), but one is not universally the optimal baseline.[Section 4, Theorem 2 and footnote 3](../../../../../gradient-estimation-using-stochastic-computation-graphs-by-john-schulman-and-others.md)

For a concrete check, take $q_\lambda(D,Z)=\operatorname{Bernoulli}(q)\,N(m,\sigma^2)$ with $q=(1+e^{-a})^{-1}$ and $\sigma=e^\ell$, and a fixed target $p(D,Z)=\operatorname{Bernoulli}(0.4)\,N(D,1)$. Direct integration gives

$$
\mathcal L=-D_{\rm KL}(\operatorname{Bern}(q)\Vert\operatorname{Bern}(0.4))-\tfrac12\{\sigma^2+m^2-2mq+q-1-2\ell\}.
$$

Using $Z=m+\sigma\varepsilon$, $\varepsilon\sim N(0,1)$, the combined integrand has components $(D-q)(W-1)$, $D-Z$ and $1-(Z-D)\sigma\varepsilon$. Their [expectations](../../../../../expected-value-split.md) are respectively $q(1-q)[\log(0.4/0.6)-\log(q/(1-q))+m-1/2]$, $q-m$ and $1-\sigma^2$, matching direct differentiation. Dropping the discrete [score function](../../../../../informant-function.md) term would incorrectly give zero for the first component. This calculation checks the combination without accepting the printed reversal.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
