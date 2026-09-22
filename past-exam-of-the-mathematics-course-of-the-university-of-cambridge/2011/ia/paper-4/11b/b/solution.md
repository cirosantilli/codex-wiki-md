<h1 id="11b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Now $\dot m=\beta$ and $\dot M=\alpha-\beta$, so

$$
M(t)=M_0+(\alpha-\beta)t,\qquad
M\dot v+\alpha v=u\beta.
$$

For $\alpha>0$, set $w=u\beta-\alpha v$. Then $\dot w=-\alpha w/M$ and $w(0)=u\beta$. For $\alpha\ne\beta$, integration gives

$$
w=u\beta\exp\left(-\alpha\int_0^t\frac{ds}{M(s)}\right)
=u\beta\left(\frac{M}{M_0}\right)^{\alpha/(\beta-\alpha)}.
$$

Consequently

$$
\boxed{v=\frac{u\beta}{\alpha}
\left[1-\left(\frac{M}{M_0}\right)^{\alpha/(\beta-\alpha)}\right].}
$$

This solution of the [rocket equation with stationary mass accretion](../../../../../../rocket-equation-with-stationary-mass-accretion.md) covers increasing or decreasing rocket mass, as long as $M>0$. For [equal-rate rocket burning and accretion](../../../../../../equal-rate-rocket-burning-and-accretion.md), in the case $\alpha=\beta>0$, the mass is constant and the linear equation instead gives

$$
\boxed{v(t)=u\left(1-e^{-\alpha t/M_0}\right).}
$$

It is also the continuous equal-rate limit of the preceding expression when written in terms of $t$.

For the no-accretion limit, expand the power as an exponential:

$$
\left(\frac{M}{M_0}\right)^{\alpha/(\beta-\alpha)}
=1+\frac{\alpha}{\beta}\log\frac{M}{M_0}+O(\alpha^2).
$$

Substitution gives

$$
\boxed{\lim_{\alpha\to0}v=u\log\frac{M_0}{M},}
$$

recovering (a). At a fixed time with $M_0-\beta t>0$, the limiting mass is $M=M_0-\beta t$, so the same calculation recovers the time-dependent no-dust solution.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11B](../../11b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
