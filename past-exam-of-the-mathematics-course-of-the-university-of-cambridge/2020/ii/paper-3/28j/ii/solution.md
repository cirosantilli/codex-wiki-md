<h1 id="28j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $L(t)=f(x,t)$ be the [likelihood function](../../../../../../likelihood-function.md). Since the [prior distribution](../../../../../../prior-probability.md) is $N(0,I_p)$, the [posterior density](../../../../../../posterior-density.md) has the form

$$
\mu(t)=\frac1ZL(t)\phi(t),
\qquad
\phi(t)=(2\pi)^{-p/2}e^{-\lVert t\rVert^2/2},
$$

where $Z$ is the [normalizing constant](../../../../../../bayesian-model-evidence.md).

Choose $0<\delta\leq1/2$ and use the [Gaussian autoregressive proposal reversible with respect to a standard normal distribution](../../../../../../gaussian-autoregressive-proposal-reversible-with-respect-to-a-standard-normal-distribution.md)

$$
s=\sqrt{1-2\delta}\,t+\sqrt{2\delta}\,Z_0,
\qquad Z_0\sim N(0,I_p).
$$

Thus

$$
q(\mathord\cdot\mid t)
=N\!\left(\sqrt{1-2\delta}\,t,2\delta I_p\right),
$$

whose [covariance matrix](../../../../../../covariance-matrix.md) is the required $2\delta I_p$. Reversibility with respect to the [standard normal distribution](../../../../../../standard-normal-distribution.md) says

$$
\phi(t)q(s\mid t)=\phi(s)q(t\mid s),
$$

so

$$
\frac{q(t\mid s)}{q(s\mid t)}=\frac{\phi(t)}{\phi(s)}.
$$

The [Metropolis–Hastings acceptance probability](../../../../../../metropolis-hastings-acceptance-probability.md) therefore reduces to

$$
\rho(t,s)
=\min\left\{
\frac{L(s)\phi(s)}{L(t)\phi(t)}
\frac{\phi(t)}{\phi(s)},1
\right\}
=\boxed{\min\left\{\frac{f(x,s)}{f(x,t)},1\right\}}.
$$

This is the [Preconditioned Crank–Nicolson algorithm](../../../../../../preconditioned-crank-nicolson-algorithm.md) with proposal scale $\beta=\sqrt{2\delta}$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [28J](../../28j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
