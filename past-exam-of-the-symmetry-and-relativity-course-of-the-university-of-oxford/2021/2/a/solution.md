<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $z^\mu(\tau)$ be the point [electric charge](../../../../electric-charge-split.md)'s [world line](../../../../world-line.md), with [proper time](../../../../proper-time.md) $\tau$ and [four-velocity](../../../../four-velocity.md) $U^\mu=dz^\mu/d\tau=\gamma(c,\mathbf u)$. For the field event $x^\mu$, choose the **retarded** source event: $R^\mu=x^\mu-z^\mu(\tau_{\rm ret})$ is future-directed and null. Write $R^\mu=(R,R\mathbf n)$, where $R=|\mathbf x-\mathbf z(t_{\rm ret})|=c(t-t_{\rm ret})$. In the instantaneous rest [inertial frame](../../../../inertial-frame.md) of that source event,

$$
U'^\mu=(c,\mathbf0),\qquad -R'_\mu U'^\mu=cR',\qquad
A'^\mu=\left(\frac{q}{4\pi\epsilon_0cR'},\mathbf0\right).
$$

Consequently the covariant expression matching this [Coulomb potential](../../../../coulomb-potential-energy.md) is

$$
\boxed{A^\mu(x)=\frac{q}{4\pi\epsilon_0}\frac{U^\mu/c}{-R_\nu U^\nu}\bigg|_{\rm ret}.}
$$

The denominator is a [Lorentz scalar](../../../../lorentz-scalar.md), so the right-hand side is a [four-vector](../../../../four-vector.md) with the required instantaneous-rest components. This describes the [retarded potential](../../../../retarded-potential.md) in [Lorenz gauge](../../../../lorenz-gauge-condition.md), with no added free [electromagnetic wave](../../../../electromagnetic-wave-split.md). [Lorentz covariance](../../../../lorentz-covariance.md) alone does not establish the boundary conditions or exclude additional terms depending on [four-acceleration](../../../../four-acceleration.md). The physical input is the retarded point-source solution of [Maxwell equations](../../../../maxwell-equations-split.md): the potential at the retarded event depends on the instantaneous [four-current](../../../../four-current.md), while its [derivatives](../../../../derivative.md) generate the acceleration field. Equivalently, evaluating the retarded source integral gives a Jacobian $1/(1-\mathbf n\cdot\boldsymbol\beta)$ from the light-cone constraint; this fixes that input for arbitrary smooth subluminal motion.[§1.7, equations (71)–(76): causal source integrals, with source quantities evaluated at retarded time](../../../../retarded-potentials-by-richard-fitzpatrick.md)

In any [inertial frame](../../../../inertial-frame.md), put $\boldsymbol\beta=\mathbf u/c$ and $\kappa=1-\mathbf n\cdot\boldsymbol\beta$. Then $-R\cdot U=\gamma cR\kappa$, and the [Liénard–Wiechert potential](../../../../lienard-wiechert-potential.md) is

$$
\phi=\frac{q}{4\pi\epsilon_0R\kappa},\qquad \mathbf A=\frac{\mathbf u}{c^2}\phi.
$$

Differentiate using $\mathbf E=-\nabla\phi-\partial_t\mathbf A$ and $\mathbf B=\nabla\times\mathbf A$, including the position and time dependence of the [retarded time](../../../../retarded-time.md). For example, $\partial t_{\rm ret}/\partial t=1/\kappa$ and $\nabla t_{\rm ret}=-\mathbf n/(c\kappa)$. The resulting [Liénard-Wiechert field](../../../../lienard-wiechert-field.md) is

$$
\boxed{\mathbf E=\frac{q}{4\pi\epsilon_0}\left[
\frac{(1-\beta^2)(\mathbf n-\boldsymbol\beta)}{\kappa^3R^2}
+\frac{\mathbf n\times[(\mathbf n-\boldsymbol\beta)\times\dot{\boldsymbol\beta}]}{c\kappa^3R}
\right]_{\rm ret},\qquad
\mathbf B=\frac1c[\mathbf n\times\mathbf E]_{\rm ret}.}
$$

Here the dot denotes a [derivative](../../../../derivative.md) with respect to source coordinate time. The first term is the velocity or non-radiative field: it falls as $R^{-2}$ and exists even without [acceleration](../../../../acceleration.md). The second is the acceleration or [radiation field](../../../../radiation-field.md), falling as $R^{-1}$ and transverse to $\mathbf n$. Its [Poynting flux](../../../../poynting-flux.md) falls as $R^{-2}$, so its outward [power](../../../../power.md) integrated over a large sphere stays finite as its radius tends to infinity. The first term's squared-field flux instead vanishes in that limit. This large-distance distinction defines [radiation](../../../../radiation.md); a moving near field can carry local [energy](../../../../energy-split.md) without constituting radiation escaping to infinity.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
