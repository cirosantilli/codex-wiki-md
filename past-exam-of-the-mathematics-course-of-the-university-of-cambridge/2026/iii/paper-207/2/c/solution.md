<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For transition-intensity vector $q$ and generator $Q(q)$, the expected infectious occupancy over three months from $S$ is the [Markov reward model](../../../../../../markov-reward-model.md) quantity

$$
m(q)=\mathbb E_S\int_0^3\mathbf1_{\{X_t=I\}}dt
=\int_0^3[e^{Q(q)t}]_{SI}\,dt.
$$

Insert the fitted intensities to obtain $m(\widehat q)$, evaluating the matrix exponential and integral numerically if necessary.

If $\eta=(\log q_{SE},\log q_{EI},\log q_{IR})$ has estimated covariance $V$, calculate the numerical gradient $g=\nabla_\eta m(e^\eta)$ at $\widehat\eta$. The [delta method](../../../../../../delta-method.md) gives estimated variance $g^TVg$ and the approximate confidence interval

$$
m(\widehat q)\pm z_{1-\alpha/2}\sqrt{g^TVg}.
$$

Simulation from $N(\widehat\eta,V)$ followed by transformation through $m$ gives a useful asymmetric alternative.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
