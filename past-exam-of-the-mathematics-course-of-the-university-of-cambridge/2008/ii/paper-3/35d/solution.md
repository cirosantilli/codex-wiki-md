<h1 id="35d/solution">Solution</h1>

↑ **Parent:** [35D](../35d.md)

The [retarded potential](../../../../../retarded-potential.md) represents causal propagation: each source element contributes according to its charge density at the earlier time needed for a signal to reach the observer, with inverse-distance weighting. The printed formula uses units with the speed of light equal to one.

Insert a [Dirac delta function](../../../../../dirac-delta-function.md) in time to write

$$
\phi(t,x)=\frac1{4\pi\epsilon_0}\int d^3x'\int d\tau\,\frac{\rho(\tau,x')}{|x-x'|}\delta(t-\tau-|x-x'|).
$$

For the moving point charge, spatial integration leaves $q/(4\pi\epsilon_0)$ times $\int R(\tau)^{-1}\delta(t-\tau-R(\tau))\,d\tau$, with $R(\tau)=|x-x_0(\tau)|$. The retarded time $\tau_r$ solves $t-\tau_r=R(\tau_r)$. Since $R'(\tau)=-v(\tau)\cdot n(\tau)$, the delta-function Jacobian is $1-v\cdot n$, positive for subluminal motion. Therefore the [Liénard–Wiechert potential](../../../../../lienard-wiechert-potential.md) is

$$
\boxed{\phi(t,x)=\frac q{4\pi\epsilon_0(R-v\cdot R)},}
$$

where $R=x-x_0(\tau_r)$ and $v=\dot x_0(\tau_r)$. Replacing charge density by the current density $qv\delta^{(3)}(x-x_0)$ gives $\boxed{A=v\phi}$ in these $c=1$ units. Restoring SI units gives denominator $R-v\cdot R/c$ and $A=v\phi/c^2$, with all source quantities still evaluated at retarded time.

## ↑ Ancestors (10)

1. [35D](../35d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
