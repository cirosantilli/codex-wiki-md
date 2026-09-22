<h1 id="35e/solution">Solution</h1>

↑ **Parent:** [35E](../35e.md)

The metric is nonsingular on $r>0$; $r=0$ is a coordinate boundary at which the displayed coefficients diverge. The nonzero [Christoffel symbols](../../../../../christoffel-symbol.md) are

$$
\Gamma^t_{tr}=\Gamma^t_{rt}=-1/r,\qquad \Gamma^r_{tt}=-1/r,\qquad \Gamma^r_{rr}=-1/r.
$$

Writing dots for derivatives with respect to [proper time](../../../../../proper-time.md), the [geodesic equations](../../../../../geodesic-equation.md) are

$$
\boxed{\ddot t-2\dot t\dot r/r=0,\qquad \ddot r-(\dot t^2+\dot r^2)/r=0.}
$$

The first gives $\dot t=kr^2$ for a constant $k$, chosen positive for a future-directed particle. Normalization of a timelike four-velocity gives $(-\dot t^2+\dot r^2)/r^2=-1$, so $\dot r^2=k^2r^4-r^2$. Dividing by $\dot t^2$ gives

$$
\boxed{(dr/dt)^2=1-1/(k^2r^2).}
$$

Integrating on each side of the turning point yields $\sqrt{r^2-k^{-2}}=|t-t_0|$, hence $r^2-(t-t_0)^2=k^{-2}$. Choose $t_0=0$ and let $\tau=0$ at the minimum radius. Then

$$
\boxed{kr=\sec\tau,\qquad kt=\tan\tau,\qquad -\pi/2<\tau<\pi/2.}
$$

Differentiating verifies $\dot t=\sec^2\tau/k=kr^2$, the normalization and the radial [Geodesic equation](../../../../../geodesic-equation.md). [proper time](../../../../../proper-time.md) therefore remains finite as the coordinate radius and time tend to infinity at the endpoints of this chart.

## ↑ Ancestors (10)

1. [35E](../35e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
