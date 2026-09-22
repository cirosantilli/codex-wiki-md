<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For smooth [vorticity](../../../../../../vorticity.md), parts (b)--(c) and the [transport equation](../../../../../../transport-equation.md) give $\omega(t,S_{0,t}(y))=\omega_{\mathrm{in}}(y)$ and measure preservation. The [change of variables formula](../../../../../../change-of-variables-formula.md) therefore conserves $\|\omega(t)\|_1$ and $\|\omega(t)\|_\infty$. Parts (d)--(e) give a uniformly bounded velocity and a uniform [log-Lipschitz modulus](../../../../../../log-lipschitz-modulus.md); applying the time-dependent version of part (f) constructs unique global [characteristic curves](../../../../../../characteristic-curve.md).

For a rough [Yudovich characteristic flow](../../../../../../yudovich-characteristic-flow.md), state the needed temporal hypothesis explicitly:

$$
\omega\in L^\infty_{\mathrm{loc}}([0,\infty);L^1\cap L^\infty),
\qquad
t\longmapsto U[\omega(t)]\ \text{measurable}.
$$

The usual weak Euler solution class provides these conditions and the initial time trace. On $[0,T]$, put $A(t)=\|\omega(t)\|_1+\|\omega(t)\|_\infty$. The velocity bounds are $|u(t,x)|\leq CA(t)$ and $|u(t,x)-u(t,y)|\leq CA(t)\mu(|x-y|)$, with $A$ integrable on this interval.

For completeness, mollify $u$ spatially. The resulting smooth velocities have trajectories and obey the same speed and modulus bounds, up to one common constant. Their speeds have the integrable majorant $CA(t)$, giving uniform boundedness and equicontinuity of trajectories. [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) supplies a uniformly convergent subsequence. The modulus estimate controls $u(t,X_\varepsilon)-u(t,X)$, while the spatial mollification error tends to zero with an integrable majorant. Thus the limit solves

$$
X(t)=y+\int_0^t u(s,X(s))\,ds.
$$

Replace $Ct$ by $C\int_0^tA(s)\,ds$ in the [Osgood uniqueness criterion](../../../../../../osgood-uniqueness-criterion.md) proof. It gives uniqueness and prevents finite-time escape. **The characteristics are globally uniquely defined for each given Euler solution in the usual Yudovich class.** This constructs the flow for a fixed solution; it is not by itself the entire uniqueness proof for the nonlinear Euler equation.

Merely saying that both spatial norms are finite separately at each time does not state the local temporal bound or measurability used in this argument. The printed formulation must be interpreted in the usual solution class, or supplemented with these temporal conditions. Also, an initial datum here is a function of $x\in\mathbb R^2$; the extra time variable in the displayed initial-data space is extraneous.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
