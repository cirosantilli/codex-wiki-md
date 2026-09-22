<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The time-translation [Killing vector field](../../../../killing-vector-field-split.md) of the [Schwarzschild metric](../../../../schwarzschild-spacetime-split.md) gives a conserved [Killing energy](../../../../killing-energy.md) per unit [rest mass](../../../../invariant-mass.md),

$$
\mathcal E=-g_{tt}\frac{dt}{d\tau}=c^2f(r)\frac{dt}{d\tau}.
$$

For unit [rest mass](../../../../invariant-mass.md), this is the total [energy](../../../../energy-split.md) relative to infinity, including [rest energy](../../../../rest-energy.md). At release $dr/d\tau=0$, so the [four-velocity](../../../../four-velocity.md) normalization gives $dt/d\tau=f(r_0)^{-1/2}$ and

$$
\boxed{\mathcal E=c^2\sqrt{1-\frac{2GM}{r_0c^2}}
=c^2-\frac{GM}{r_0}+O\left(\frac{G^2M^2}{r_0^2c^2}\right).}
$$

Substitution into the radial [four-velocity](../../../../four-velocity.md) normalization yields

$$
\left(\frac{dr}{d\tau}\right)^2=\frac{\mathcal E^2}{c^2}-c^2f(r)
=2GM\left(\frac1r-\frac1{r_0}\right).
$$

Choosing the inward square root and evaluating at the ground proves

$$
\boxed{\frac12\left(\frac{dr}{d\tau}\right)^2_{r=R_E}
=GM\left(\frac1{R_E}-\frac1{R_E+h}\right).}
$$

This identity is exact within the assumed [Schwarzschild metric](../../../../schwarzschild-spacetime-split.md), despite its familiar [Newtonian mechanics](../../../../newtonian-mechanics-split.md) form. The quantity $dr/d\tau$ is not exactly the locally measured [speed](../../../../speed.md). A [Schwarzschild static observer](../../../../schwarzschild-static-observer.md) measures $v_{\rm loc}=(dr/dt)/f=(dr/d\tau)/\sqrt{f(r_0)}$. Thus the distinction disappears in the stated [weak-field approximation](../../../../weak-field-approximation.md), giving $v_{\rm loc}^2\simeq2gh$ for $h\ll R_E$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
