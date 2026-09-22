<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V=U-c$ and take $k>0$ without loss of generality. The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) replaces density by $\rho_0$ in inertia and pressure acceleration, while retaining the density perturbation in [buoyancy](../../../../../../buoyancy.md). Linearizing about the [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) and substituting the [normal mode](../../../../../../normal-mode.md) gives

$$
ikV\widehat u+U'\widehat w=-ik\widehat p/\rho_0,\qquad
ikV\widehat w=-\widehat p'/\rho_0-g\widehat\rho/\rho_0,
$$



$$
ik\widehat u+\widehat w'=0,\qquad
ikV\widehat\rho+\rho'\widehat w=0.
$$

The last two equations give $\widehat u=i\widehat w'/k$ and $\widehat\rho=i\rho'\widehat w/(kV)$. The horizontal momentum equation gives

$$
\frac{\widehat p}{\rho_0}=\frac{V\widehat w'-U'\widehat w}{ik}.
$$

Substituting in the vertical momentum equation yields the [Taylor–Goldstein equation](../../../../../../taylor-goldstein-equation.md):

$$
\boxed{\widehat w''-k^2\widehat w-\frac{U''}{U-c}\widehat w+\frac{N^2}{(U-c)^2}\widehat w=0,\qquad
N^2=-\frac g{\rho_0}\rho'.}
$$

The [buoyancy frequency](../../../../../../buoyancy-frequency.md) is real for [stable density stratification](../../../../../../stable-density-stratification.md). The impermeable walls impose $\widehat w(\pm L)=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
