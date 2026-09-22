<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $\tau=T-t$, $\kappa=\lambda-\rho b\theta$ and $k=\theta(\theta-1)/2$. For the [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md) volatility, the transformed [partial differential equation](../../../../../../partial-differential-equation-split.md) is

$$
V_\tau=\frac12b^2V_{\sigma\sigma}+(\lambda a-\kappa\sigma)V_\sigma+k\sigma^2V.
$$

Use the [Gaussian volatility exponential-quadratic transform](../../../../../../gaussian-volatility-exponential-quadratic-transform.md) ansatz $V=\exp(P+Q\sigma+R\sigma^2)$, where the coefficients depend on $\tau$. Its derivatives satisfy

$$
V_\sigma/V=Q+2R\sigma,\qquad
V_{\sigma\sigma}/V=2R+(Q+2R\sigma)^2,\qquad
V_\tau/V=\dot P+\dot Q\sigma+\dot R\sigma^2.
$$

Matching the constant, linear and quadratic powers of $\sigma$ gives

$$
\boxed{\begin{aligned}
F(R)&=2b^2R^2-2(\lambda-\rho b\theta)R+\tfrac12\theta(\theta-1),\\
G(Q,R)&=\{2b^2R-(\lambda-\rho b\theta)\}Q+2\lambda aR,\\
H(Q,R)&=b^2R+\tfrac12b^2Q^2+\lambda aQ.
\end{aligned}}
$$

The terminal condition requires

$$
\boxed{P(0)=Q(0)=R(0)=0.}
$$

These polynomial [ordinary differential equations](../../../../../../ordinary-differential-equation.md) have a unique local solution by the [Picard's theorem for ordinary differential equations](../../../../../../picard-lindelof-theorem.md). Substitution then proves the desired [partial differential equation](../../../../../../partial-differential-equation-split.md) solution on every horizon for which the coefficient solution remains finite. The [Riccati equation](../../../../../../riccati-equation.md) for $R$ is solved first; $Q$ subsequently solves a linear equation and $P$ is an integral of known coefficients.

**Unrestricted global existence needs a qualification.** Take $a=0$, $\lambda=b=1$, $\rho=0$ and $\theta=2$. Then $Q=0$ and the [Riccati equation](../../../../../../riccati-equation.md) becomes

$$
\dot R=2R^2-2R+1,\qquad
R(\tau)=\frac12\left\{1+\tan(\tau-\pi/4)\right\}.
$$

This solves the initial condition but explodes at $\tau=3\pi/4$. Therefore no finite real exponential-quadratic solution with the required terminal condition exists on an entire horizon $T\ge3\pi/4$ for these allowed parameters. The correct general claim is local existence, or existence before the [Riccati moment-explosion horizon](../../../../../../riccati-moment-explosion-horizon.md).

A useful sufficient global condition is $0\le\theta\le1$, so $k\le0$. If $b\ne0$, the lower equilibrium

$$
r_-=\frac{\kappa-\sqrt{\kappa^2-2b^2k}}{2b^2}\le0
$$

traps the solution in $r_-\le R(\tau)\le0$: the polynomial vector field points inward at the upper endpoint and vanishes at the lower endpoint. If $b=0$, the equation for $R$ is linear. In either case there is no finite-time explosion; $Q$ is then a linear equation with coefficients bounded on compact time intervals, and $P$ is finite on those intervals. This proves the intended ansatz globally under that sufficient parameter restriction, without asserting it for every real $\theta$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
