<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a deterministic $t>0$ and define $\widehat B_u=B_{t+u}-B_t$, $\widehat H_u=H_{t+u}$ and $\widehat{\mathcal F}_u=\mathcal F_{t+u}$. The increment process is a standard [Brownian motion](../../../../../../brownian-motion-split.md) in the shifted filtration, and $\widehat H$ remains bounded, continuous and adapted. Thus part (a) applies even though the initial value $\widehat H_0=H_t$ is random. For $\varepsilon>0$,

$$
\frac{\int_t^{t+\varepsilon}H_s\,dB_s}{B_{t+\varepsilon}-B_t}-H_t
=\frac{\int_t^{t+\varepsilon}(H_s-H_t)\,dB_s}{B_{t+\varepsilon}-B_t}.
$$

Here the constant-in-time integrand $H_t$ is $\mathcal F_t$-measurable, so its [stochastic integral](../../../../../../stochastic-integral.md) equals $H_t(B_{t+\varepsilon}-B_t)$. The expectation of the absolute value of the right-hand side to the power $1/4$ tends to zero by part (a). For every $\eta>0$, [Markov inequality](../../../../../../markov-inequality.md) consequently gives

$$
\mathbb P\left(\left|\frac{\int_t^{t+\varepsilon}H_s\,dB_s}{B_{t+\varepsilon}-B_t}-H_t\right|>\eta\right)
\leq\eta^{-1/4}\mathbb E\left|\frac{\int_t^{t+\varepsilon}(H_s-H_t)\,dB_s}{B_{t+\varepsilon}-B_t}\right|^{1/4}\longrightarrow0.
$$

Therefore

$$
\boxed{\frac1{B_{t+\varepsilon}-B_t}\int_t^{t+\varepsilon}H_s\,dB_s\xrightarrow[\varepsilon\downarrow0]{\mathbb P}H_t\quad\text{for every fixed }t>0.}
$$

The stated [convergence in probability](../../../../../../convergence-in-probability.md) holds for each fixed deterministic time.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
