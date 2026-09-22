<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a stationary linear autoregression, [causal time series](../../../../../../causal-time-series.md) means that the observation uses only current and past driving noise:

$$
Y_t=\sum_{j\geq0}\psi_j\varepsilon_{t-j},\qquad \sum_{j\geq0}|\psi_j|^2<\infty.
$$

This is a convergent in the sense of [mean-square convergence](../../../../../../convergence-in-l2.md) [infinite moving-average representation](../../../../../../infinite-moving-average-representation.md). The stronger usual stable-filter definition requires absolute summability; the argument below also handles the square-summable definition. Let $\Phi(z)=1-\sum_{k=1}^p\phi_kz^k$ and $\Psi(z)=\sum_{j\geq0}\psi_jz^j$. Substituting the filter into the recurrence and comparing coefficients of the orthogonal noise gives $\psi_0=1$ and $\psi_j=\sum_{k=1}^{\min(p,j)}\phi_k\psi_{j-k}$. Hence

$$
\Phi(z)\Psi(z)=1\qquad(|z|<1).
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) ensures that $\Psi$ is an [analytic function](../../../../../../space-of-holomorphic-functions.md) in this disk. Thus $\Phi$ has no zero strictly inside it. A boundary zero is also impossible: a zero of multiplicity $m\geq1$ at $z_0=e^{i\omega_0}$ makes $|1/\Phi(re^{i\omega})|^2$ at least a constant times $[(1-r)^2+(\omega-\omega_0)^2]^{-m}$ near that point. Its integral over $\omega$ diverges as $r\uparrow1$. On the other hand, [orthogonality of complex exponentials](../../../../../../orthogonality-of-complex-exponentials.md) gives

$$
\frac1{2\pi}\int_{-\pi}^{\pi}|\Psi(re^{i\omega})|^2\,d\omega
=\sum_{j\geq0}|\psi_j|^2r^{2j}\leq\sum_{j\geq0}|\psi_j|^2<\infty,
$$

a contradiction. Therefore the [causality root criterion for an autoregressive model](../../../../../../causality-root-criterion-for-an-autoregressive-model.md) is

$$
\boxed{\Phi(z)=0\ \Longrightarrow\ |z|>1.}
$$

Under absolute summability, the shorter boundary argument is continuity of $\Psi$ on the closed disk and the identity $\Phi\Psi=1$ there.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
