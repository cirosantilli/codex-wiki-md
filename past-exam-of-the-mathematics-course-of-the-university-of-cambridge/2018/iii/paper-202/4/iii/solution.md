<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\Delta B_h=B_{t+h}-B_t$ and $R_h=\int_t^{t+h}(H_s-H_t)dB_s$. The constant-in-time coefficient $H_t$ on $(t,t+h]$ is [previsible](../../../../../../predictable-process.md), so the ratio minus $H_t$ is $R_h/\Delta B_h$. Since $|H|\leq C$, continuity and the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) imply

$$
\eta_h=\mathbb E\sup_{t\leq s\leq t+h}|H_s-H_t|^2\longrightarrow0.
$$

The [Itô isometry](../../../../../../ito-isometry.md) gives $\mathbb ER_h^2\leq h\eta_h$. For $\varepsilon,\delta>0$, use the [Chebyshev inequality](../../../../../../chebyshev-inequality.md) and the [normal distribution](../../../../../../normal-distribution.md) of $\Delta B_h/\sqrt h$ to obtain

$$
\mathbb P\left(\left|\frac{R_h}{\Delta B_h}\right|>\varepsilon\right)
\leq\mathbb P(|N(0,1)|\leq\delta)+\frac{\eta_h}{\varepsilon^2\delta^2}.
$$

First let $h\downarrow0$, then $\delta\downarrow0$; the [normal distribution](../../../../../../normal-distribution.md) has no atom at zero. This proves

$$
\boxed{\frac{\int_t^{t+h}H_s\,dB_s}{B_{t+h}-B_t}\xrightarrow[h\downarrow0]{\mathbb P}H_t.}
$$

No [independence](../../../../../../independent-random-variables.md) between $R_h$ and the denominator is needed.

The first estimate suggested by the hint is valid: [Brownian scaling](../../../../../../brownian-scaling.md) and the [Gamma function](../../../../../../gamma-function.md) give $\mathbb E|\Delta B_h|^{-1/2}=h^{-1/4}2^{-1/4}\Gamma(1/4)/\sqrt\pi$. The second hint requires care about the placement of its [expectation](../../../../../../expected-value.md): with $V_h=\int_t^{t+h}(H_s-H_t)^2ds$, the interpretation $\mathbb E|R_h|^{1/2}\leq(\mathbb EV_h)^{1/4}$ is correct by the [Jensen inequality](../../../../../../jensen-s-inequality.md) and the [Itô isometry](../../../../../../ito-isometry.md), whereas **the interpretation $\mathbb E|R_h|^{1/2}\leq\mathbb E(V_h^{1/4})$ is false with constant $1$**. For the latter interpretation, the [Burkholder-Davis-Gundy inequality](../../../../../../burkholder-davis-gundy-inequalities.md) supplies a constant $C_{1/2}$ instead. One can see the obstruction with a [Brownian motion](../../../../../../brownian-motion-split.md) stopped on exiting $(-1,1)$: if $\tau$ is that [Brownian exit time](../../../../../../brownian-exit-time.md), then $|B_\tau|=1$, $\mathbb E\tau=1$, and strict [Jensen inequality](../../../../../../jensen-s-inequality.md) gives $\mathbb E\tau^{1/4}<1=\mathbb E|B_\tau|^{1/2}$.

This obstruction also survives the continuity condition on $H$. On a long finite interval approximate $\mathbf1_{\{s<\tau\}}$ by a continuous [adapted process](../../../../../../adapted-process.md) equal to $1$ until $\tau$ and decreasing linearly to $0$ during the next $\epsilon$ units of time, and take its initial value to be $0$ by inserting a short continuous ramp before starting the exit experiment. The [Itô isometry](../../../../../../ito-isometry.md) controls these approximations, and letting the interval length tend to infinity recovers the strict inequality above; hence some bounded continuous [adapted](../../../../../../adapted-process.md) example also violates the latter interpretation with constant $1$. The direct proof avoids relying on this ambiguous hint.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
