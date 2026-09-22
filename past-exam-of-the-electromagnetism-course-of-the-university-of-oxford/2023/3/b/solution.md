<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The moving [point charge](../../../../point-charge.md) has distributional [charge density](../../../../charge-density.md) and [current density](../../../../current-density.md)

$$
\rho(\mathbf r',t')=q\delta^{(3)}(\mathbf r'-\mathbf r_0(t')),\qquad
\mathbf J(\mathbf r',t')=q\mathbf v_0(t')\delta^{(3)}(\mathbf r'-\mathbf r_0(t')).
$$

Let

$$
K(\mathbf r,t;\mathbf r',t')=
\frac{\delta(t-t'-|\mathbf r-\mathbf r'|/c)}{|\mathbf r-\mathbf r'|}.
$$

The given [retarded fundamental solution](../../../../retarded-fundamental-solution.md) identity immediately implies that the [retarded potentials](../../../../retarded-potential.md)

$$
\phi=\frac1{4\pi\epsilon_0}\int K\rho\,d^3r'\,dt',\qquad
\mathbf A=\frac{\mu_0}{4\pi}\int K\mathbf J\,d^3r'\,dt'
$$

solve $\square\phi=-\rho/\epsilon_0$ and $\square\mathbf A=-\mu_0\mathbf J$ in the sense of [distributions](../../../../distribution-mathematical-analysis.md). Integrating the spatial [Dirac delta function](../../../../dirac-delta-function.md) first gives

$$
\phi=\frac q{4\pi\epsilon_0}\int_{-\infty}^{\infty}
\frac{\delta(g(t'))}{R(t')}\,dt',\qquad
g(t')=t-t'-R(t')/c,
$$

and the analogous integral for $\mathbf A$ has numerator $\mu_0q\mathbf v_0(t')/(4\pi)$.

Assume the physical trajectory has [subluminal speed](../../../../subluminal-speed.md) and the [retarded time](../../../../retarded-time.md) exists. At its root $t_r$, with $\mathbf n_r=\mathbf R(t_r)/R(t_r)$,

$$
\frac{dR}{dt'}=-\frac{\mathbf R\cdot\mathbf v_0}{R},\qquad
g'(t_r)=-\left(1-\frac{\mathbf n_r\cdot\mathbf v_0(t_r)}c\right).
$$

The positive factor $\kappa=1-\mathbf n_r\cdot\mathbf v_0/c$ also proves [uniqueness of retarded time for a subluminal source](../../../../uniqueness-of-retarded-time-for-a-subluminal-source.md). The [Dirac delta function](../../../../dirac-delta-function.md) substitution formula gives $\delta(g(t'))=\delta(t'-t_r)/\kappa$, so

$$
\boxed{\phi(\mathbf r,t)=\frac q{4\pi\epsilon_0}
\frac1{R(t_r)-\mathbf R(t_r)\cdot\mathbf v_0(t_r)/c},\qquad
\mathbf A(\mathbf r,t)=\frac{\mathbf v_0(t_r)}{c^2}\phi(\mathbf r,t).}
$$

These are the [Liénard–Wiechert potentials](../../../../lienard-wiechert-potential.md). The denominator includes the time-substitution factor, rather than just the retarded distance. Away from the trajectory the [electric potential](../../../../electric-potential.md) and [magnetic vector potential](../../../../magnetic-vector-potential.md) are ordinary smooth functions; on the trajectory their [wave equations](../../../../wave-equation-split.md) have the indicated distributional sources.

For completeness, the [charge continuity equation](../../../../charge-continuity-equation.md) $\partial_{t'}\rho+\nabla'\cdot\mathbf J=0$ also verifies the [Lorenz gauge](../../../../lorenz-gauge-condition.md). Using $\nabla K=-\nabla'K$ and $\partial_tK=-\partial_{t'}K$, [integration by parts](../../../../integration-by-parts.md) in the retarded integrals gives

$$
\nabla\cdot\mathbf A+c^{-2}\partial_t\phi
=\frac{\mu_0}{4\pi}\int K(\nabla'\cdot\mathbf J+\partial_{t'}\rho)\,d^3r'\,dt'=0,
$$

with the retarded boundary prescription. Thus the construction also has the required [Lorenz gauge condition](../../../../lorenz-gauge-condition.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the electromagnetism course of the University of Oxford](../../../split.md)
5. [Electromagnetism course of the University of Oxford](../../../../electromagnetism-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
