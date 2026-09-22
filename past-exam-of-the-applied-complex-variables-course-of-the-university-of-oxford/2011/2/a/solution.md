<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\zeta=\zeta(z,t)$ be the inverse [conformal map](../../../../conformal-map.md). With $Q$ real and nonzero, the [function](../../../../function-split.md) $Q\log|\zeta|$ is [harmonic](../../../../harmonic-function.md) away from the source, vanishes on the moving [boundary](../../../../boundary-of-a-set.md), and has the required logarithmic [singularity](../../../../complex-singularity.md). Indeed $F(\zeta,t)=a_1(t)\zeta+O(\zeta^2)$ with $a_1\ne0$, so $\log|\zeta|=\log|z|-\log|a_1|+o(1)$ near the origin. Subtracting this candidate from the physical [velocity potential](../../../../velocity-potential.md) leaves a bounded [harmonic function](../../../../harmonic-function.md) near the source. Its [singularity](../../../../complex-singularity.md) is removable, and the difference has zero [boundary values](../../../../boundary-value.md). The [maximum principle for harmonic functions](../../../../maximum-principle-for-harmonic-functions.md) makes it identically zero. Therefore

$$
\boxed{\phi(z,t)=Q\log|\zeta(z,t)|=\operatorname{Re}\bigl(Q\operatorname{Log}\zeta(z,t)\bigr).}
$$

Only the [real part](../../../../real-part.md) is needed, so the multivalued [imaginary part](../../../../imaginary-part.md) of the logarithm causes no ambiguity in $\phi$.

Differentiate $F(\zeta(z,t),t)=z$ while holding the physical point $z$ fixed:

$$
\zeta_t=-\frac{F_t}{F_\zeta},\qquad
\phi_t=-Q\operatorname{Re}\frac{F_t}{\zeta F_\zeta}.
$$

Also the local analytic [complex potential of a two-dimensional potential flow](../../../../complex-potential-of-a-two-dimensional-potential-flow.md) has [derivative](../../../../derivative.md)

$$
w_z=\frac{Q}{\zeta F_\zeta},\qquad |\nabla\phi|^2=|w_z|^2=\frac{Q^2}{|\zeta F_\zeta|^2}.
$$

The distinction between differentiating at fixed $z$ and fixed $\zeta$ is essential because the [boundary](../../../../boundary-of-a-set.md) map depends on time. Substituting into the [boundary](../../../../boundary-of-a-set.md) evolution law and multiplying by $|\zeta F_\zeta|^2/Q$ gives

$$
\operatorname{Re}\bigl(F_t\overline{\zeta F_\zeta}\bigr)=Q.
$$

Taking the conjugate inside a [real part](../../../../real-part.md) leaves it unchanged, so the desired [conformal map equation for planar Darcy growth](../../../../conformal-map-equation-for-planar-darcy-growth.md) is

$$
\boxed{\operatorname{Re}\left(\zeta F_\zeta\overline{F_t}\right)=Q,\qquad |\zeta|=1.}
$$

As a normalization check, parameterize the [boundary](../../../../boundary-of-a-set.md) by $\zeta=e^{i\theta}$. Its outward [normal vector](../../../../normal-vector.md) times arclength is $\zeta F_\zeta\,d\theta$, so its [area](../../../../surface-area.md) growth rate is $\int_0^{2\pi}\operatorname{Re}(F_t\overline{\zeta F_\zeta})d\theta=2\pi Q$, exactly the specified source [flux](../../../../flux.md). For an expanding circular map $F=R(t)\zeta$, the equation reduces to $R\dot R=Q$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the applied complex variables course of the University of Oxford](../../../split.md)
5. [Applied complex variables course of the University of Oxford](../../../../applied-complex-variables-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
