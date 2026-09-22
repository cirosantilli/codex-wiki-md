<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Bedload transport](../../../../bedload-transport.md) carries sediment by rolling, sliding and short hops near the bed. [Suspended sediment](../../../../suspended-sediment.md) is held in the water column by turbulent mixing. The competition between particle [settling velocity](../../../../settling-velocity.md) and the turbulent vertical velocity scale chiefly determines which description applies; particle size and density influence that settling velocity.

Scale the depths and bed/free-surface elevations by $d$, both velocities by $U$, distance by $L$, and time by $T$. A choice producing exactly the requested coefficients is

$$
\boxed{U=\sqrt{\frac{gSd}{f}},\quad L=\frac{\rho_sa}{f\rho_w},\quad T=\frac{dL}{aU}.}
$$

The sediment continuity equation then has unit coefficients, while both material-acceleration time derivatives acquire the factor $L/(UT)=a/d$. Dividing water momentum by $gd/L$ and sediment momentum by $U^2/L$ gives

$$
\boxed{\varepsilon=\frac ad,\quad F^2=\frac{U^2}{gd}=\frac Sf,\quad
\delta=\frac{SL}{d}=\frac{\rho_s}{\rho_w}\varepsilon F^2,\quad
\kappa=\frac{f_bL}{U}.}
$$

For example $d=1\,\mathrm m$, $a=10^{-3}\,\mathrm m$, $S=10^{-3}$, $f=10^{-2}$ and $\rho_s/\rho_w=2.65$ give $\varepsilon=10^{-3}$ and $\delta=2.65\times10^{-4}$. These are illustrative values: small effective mobile-layer thickness and small slope explain the two small parameters.

Set $\varepsilon=\delta=0$ at leading order. Water continuity gives $hu=q$, with spatially constant flux; take a prescribed constant $q$. Water momentum integrates to $\eta+F^2u^2/2=C$. Since $s=\eta-h$,

$$
\boxed{s(u)=C-\frac{F^2u^2}{2}-\frac qu.}
$$

The [bedload transport model with sediment inertia](../../../../bedload-transport-model-with-sediment-inertia.md) has remaining equations $s(u)_t+v_x=0$ and $vv_x=(u-v)^2-\kappa v$.

Choose a uniform state of this reduced model with $h_0=u_0=q=1$, constant $s_0=C-F^2/2-1$, and

$$
\boxed{v_0=\frac{2+\kappa-\sqrt{\kappa^2+4\kappa}}2\in(0,1).}
$$

It satisfies $(1-v_0)^2=\kappa v_0$. For small perturbations $U,V$ of the two velocities, put $a_1=2(1-v_0)>0$ and $b_1=a_1+\kappa>0$. [Linearization](../../../../linearization.md) gives

$$
(1-F^2)U_t+V_x=0,\qquad v_0V_x=a_1U-b_1V.
$$

For a [Fourier mode](../../../../fourier-mode.md) $e^{ikx+\lambda t}$ this yields

$$
\lambda=-\frac{ika_1}{(1-F^2)(b_1+ikv_0)},\qquad
\boxed{\operatorname{Re}\lambda=-\frac{a_1v_0k^2}{(1-F^2)(b_1^2+k^2v_0^2)}.}
$$

Every nonzero mode decays for $F<1$ and grows for $F>1$. The spatially uniform mode is neutral, and $F=1$ is a singular threshold where the neglected terms matter. In a general uniform state the controlling sign is $q/u_0^2-F^2u_0$: equivalently the actual mean-flow [Froude number](../../../../froude-number.md) is less or greater than one. The displayed $F=1$ criterion uses the stated unit-depth, unit-velocity normalization of the reduced steady state.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
