<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
y=\frac{4\pi}{\alpha_\lambda}=\frac{(4\pi)^2}{\lambda^2},\qquad t=\log\mu^2.
$$

The chain rule gives

$$
\frac{dy}{dt}=-(4\pi)^2\lambda^{-3}\beta(\lambda)=\beta_0+\frac{\beta_1}{y}+O(y^{-2}).
$$

For the [ultraviolet](../../../../../../ultraviolet.md) expansion take $\beta_0>0$ and $L=\log(\mu^2/\Lambda^2)\gg1$. The leading solution is $y\sim\beta_0L$. Substituting it in the next term gives $dy/dL=\beta_0+\beta_1/(\beta_0L)+O(\log L/L^2)$, whose integration yields

$$
\boxed{\frac{4\pi}{\alpha_\lambda}=\beta_0L+\frac{\beta_1}{\beta_0}\log L+O\!\left(\frac{\log L}{L}\right).}
$$

Choosing $\Lambda$ removes the additive constant. This proves the two displayed leading terms of the [two-loop asymptotic running coupling](../../../../../../two-loop-asymptotic-running-coupling.md).

**The printed remainder is too small in general.** This can be checked even for an exactly two-loop [renormalization-group beta function](../../../../../../beta-function-physics.md), so it does not depend on unknown higher-loop effects. Put $c=\beta_1/\beta_0$. Separating variables and fixing the integration constant gives

$$
y-c\log\!\left(\frac{y+c}{\beta_0}\right)=\beta_0L.
$$

Expanding this identity one order further gives

$$
y=\beta_0L+c\log L+\frac{c^2}{\beta_0}\frac{\log L+1}{L}+O\!\left(\frac{(\log L)^2}{L^2}\right).
$$

The $\log L/L$ term cannot be absorbed into a fixed change of $\Lambda$. For example, with $\beta_0=\beta_1=1$, the exact implicit relation is $y-\log(y+1)=L$, and the next term is $(\log L+1)/L$, which is not $O(1/L)$. The unspecified $O(y^{-2})$ contribution to the [differential equation](../../../../../../differential-equation-split.md) changes the constant coefficient of $1/L$, while the coefficient $\beta_1^2/\beta_0^3$ of $\log L/L$ is already fixed. Only special cases such as $\beta_1=0$ avoid this particular obstruction.

The asymptotic formula also presupposes an asymptotically free [ultraviolet](../../../../../../ultraviolet.md) regime. If $\beta_0=0$, division by it is invalid and the leading scaling changes. If $\beta_0<0$, the weak-coupling asymptotic direction is generally toward the [infrared](../../../../../../infrared.md) and the logarithmic variable must be chosen accordingly. These qualifications distinguish the valid perturbative solution from an unconditional formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
