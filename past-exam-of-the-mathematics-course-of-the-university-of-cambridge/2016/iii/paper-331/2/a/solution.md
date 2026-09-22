<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) with a constant inertial reference [mass density](../../../../../../density.md) $\rho_0$, keeping the background [mass density](../../../../../../density.md) gradient in [buoyancy](../../../../../../buoyancy.md). Write $V(z)=\overline U(z)-c$ and $P=\widehat p/\rho_0$. For $k\ne0$, the linearized [normal mode](../../../../../../normal-mode.md) equations are

$$
ikV\widehat u+\overline U'\widehat w=-ikP,\qquad
ikV\widehat w=-P'-\frac g{\rho_0}\widehat\rho,\qquad
ikV\widehat\rho+\overline\rho'\widehat w=0,\qquad
ik\widehat u+\widehat w'=0.
$$

The reference [mass density](../../../../../../density.md) is chosen close to the background values, whose relative variation must be small. Hydrostatic background [pressure](../../../../../../pressure.md) satisfies $\overline p'=-g\overline\rho$.

From [incompressibility](../../../../../../incompressible-flow.md), $\widehat u=i\widehat w'/k$. The horizontal momentum equation and the density equation then give

$$
P=\frac{V\widehat w'-\overline U'\widehat w}{ik},\qquad
\widehat\rho=-\frac{\overline\rho'\widehat w}{ikV}.
$$

Substitute these into the vertical momentum equation and multiply by $ik$:

$$
-k^2V\widehat w=-V\widehat w''+\overline U''\widehat w+\frac{g\overline\rho'}{\rho_0V}\widehat w.
$$

For $V\ne0$, rearrangement gives **the [Taylor–Goldstein equation](../../../../../../taylor-goldstein-equation.md)**

$$
\boxed{\widehat w''-k^2\widehat w-\frac{\overline U''}{\overline U-c}\widehat w+\frac{N^2}{(\overline U-c)^2}\widehat w=0,\qquad
N^2=-\frac g{\rho_0}\overline\rho'.}
$$

The [buoyancy frequency](../../../../../../buoyancy-frequency.md) $N$ is real for stable stratification, where $\overline\rho'<0$. Points where $\overline U=c$ are [critical levels of an internal gravity wave](../../../../../../critical-level-of-an-internal-gravity-wave.md); the derivation there is understood through a limiting or piecewise formulation. The printed density gradient is $\overline\rho'$, not the pressure gradient accidentally substituted in the local TeX.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
