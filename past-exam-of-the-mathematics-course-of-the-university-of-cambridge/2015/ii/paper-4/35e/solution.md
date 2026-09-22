<h1 id="35e/solution">Solution</h1>

↑ **Parent:** [35E](../35e.md)

To recover the printed dispersion relation, interpret the surface maintained flat as an imposed flat upper boundary for the perturbation, so its normal velocity is zero. This is the [rigid-lid approximation](../../../../../rigid-lid-approximation.md). Work with perturbation [velocity potentials](../../../../../velocity-potential.md) $\phi_-=A e^{ky}e^{ikx+\sigma t}$ below the interface and $\phi_+=B\cosh[k(y-h)]e^{ikx+\sigma t}$ in the upper layer. They solve the [Laplace equation](../../../../../laplace-equation.md), decay as $y\to-\infty$, and obey $\partial_y\phi_+(h)=0$.

The linear [kinematic boundary conditions](../../../../../kinematic-boundary-condition.md) at the interface give $(\sigma+ikU)\eta_0=kA$ and $\sigma\eta_0=-kB\sinh(kh)$. Equality of pressures, using the linear [Bernoulli equation](../../../../../bernoulli-equation.md), gives $(\sigma+ikU)A=\sigma B\cosh(kh)$. The equal fluid densities cancel the interface gravitational restoring term. Eliminating $A,B,\eta_0$ yields

$$
\boxed{(\sigma+ikU)^2+\sigma^2\coth(kh)=0.}
$$

With $q=\tanh(kh)$, the roots are

$$
\boxed{\sigma=\frac{Uk}{1+q}(-iq\pm\sqrt q),\qquad\operatorname{Re}\sigma=\pm\frac{Uk\sqrt{\tanh(kh)}}{1+\tanh(kh)}.}
$$

For every $k>0$ one root has positive real part. Thus the [vortex sheet](../../../../../vortex-sheet.md) has a [Kelvin-Helmholtz instability](../../../../../kelvin-helmholtz-instability.md) at every wavelength in this model. If $kh\gg1$, $q\to1$ and the growing rate is $Uk/2$. If $kh\ll1$, $q\sim kh$ and it is $Uk\sqrt{kh}$.

There is a physical qualification to the wording. A dynamically deformable [free surface](../../../../../free-surface.md) at finite gravity is not exactly a flat lid. Its linear conditions combine to $\sigma^2\phi_+(h)+g\partial_y\phi_+(h)=0$. Writing the upper potential as $B\cosh(ky)+C\sinh(ky)$ and using the same interface conditions instead gives

$$
(\sigma+ikU)^2[\sigma^2+gk\tanh(kh)]+\sigma^2[\sigma^2\tanh(kh)+gk]=0.
$$

The stated quadratic follows in the strong-gravity flat-surface limit, or with the flat condition imposed exactly. **It is not the exact dispersion relation of a freely moving upper surface at arbitrary finite $g$.** This makes explicit the boundary interpretation needed for the requested formula.

## ↑ Ancestors (10)

1. [35E](../35e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
