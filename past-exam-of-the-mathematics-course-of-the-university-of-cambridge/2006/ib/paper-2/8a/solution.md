<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

A [material derivative](../../../../../material-derivative.md) measures the rate experienced by a moving fluid particle. If its position is $\boldsymbol X(t)$ with $\dot{\boldsymbol X}=\boldsymbol u(\boldsymbol X,t)$, the [chain rule](../../../../../chain-rule.md) for any scalar field $F$ gives

$$
\frac d{dt}F(\boldsymbol X(t),t)=\partial_tF+\dot{\boldsymbol X}\cdot\nabla F=\partial_tF+\boldsymbol u\cdot\nabla F.
$$

Hence the operator is $D/Dt=\partial_t+\boldsymbol u\cdot\nabla$, and the [material derivative](../../../../../material-derivative.md) differs from the time derivative at a fixed spatial point.

In the steady temperature problem $\partial_t\theta=0$ and the transverse velocity vanishes. Thus at each fixed $y\in(-1,1)$,

$$
(1-y^2)\partial_x\theta=-\theta.
$$

Integrating in $x$ and applying the inlet value gives

$$
\boxed{\theta(x,y)=\theta_0\exp\left[-\frac{x}{1-y^2}\right],\qquad x>0,\ -1<y<1.}
$$

A particle's travel time from the inlet is $x/(1-y^2)$, so the formula is also the exponential decay along its [characteristic curve](../../../../../characteristic-curve.md). For fixed $x>0$ the temperature tends to zero near either wall, because the travel time becomes large. No value at $y=\pm1$ is imposed by an inlet condition there, since the wall velocity is zero and the stated channel is open in $y$.

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
