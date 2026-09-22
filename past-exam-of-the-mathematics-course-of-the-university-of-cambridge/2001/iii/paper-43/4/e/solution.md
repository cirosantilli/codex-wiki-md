<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

With inflow and overflow both zero and fixed reservoir volume $V$, the transient balances are $V\dot T=-AF_T$ and $V\dot S=-AF_S$. Therefore

$$
\frac{d\eta}{d\theta}=\frac{R_F}{R_0}=q,\qquad
\eta=\eta_s+q(\theta-\theta_s)=q\theta.
$$

The last equality uses the initial steady state. Define $k_c=Ab(\alpha T_0)^{1/3}/(V R_0^2)=CQ/V$, where the latter $Q$ is the pre-shutdown flow. The [post-shutdown double-diffusive reservoir cooling](../../../../../../post-shutdown-double-diffusive-reservoir-cooling.md) equation is

$$
\dot\theta=k_c\frac{(1-\theta)^{10/3}}{(1-q\theta)^2}.
$$

Separate variables. An explicit primitive of $(1-q\theta)^2/(1-\theta)^{10/3}$ is

$$
G(\theta)=\frac{3(1-q)^2}{7}(1-\theta)^{-7/3}
+\frac{3q(1-q)}2(1-\theta)^{-4/3}+3q^2(1-\theta)^{-1/3}.
$$

Differentiate it to verify the three powers. Hence

$$
\boxed{\eta=q\theta,\qquad t=t_0+\frac{G(\theta)-G(\theta_s)}{k_c}.}
$$

For $q<1$, $\theta$ increases monotonically to one only at infinite time, with $1-\theta\sim[3(1-q)^2/(7k_ct)]^{3/7}$ up to the choice of time origin. The reservoir approaches $T_\infty$, but its salinity tends to $S_i-qS_0$, leaving the positive salt contrast $(1-q)S_0$. Thus $R_\rho\to\infty$ and the double-diffusive flux shuts down asymptotically. The assumption of a stationary interface and continued applicability of this flux parameterization is part of the reservoir model, not a claim about every actual hydrothermal pool.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
