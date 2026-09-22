# Constant-flux tracer inlet solution

↑ **Parent:** [Advection-diffusion equation](advection-diffusion-equation.md)

For a [passive scalar](passive-scalar.md) on a half-line, impose constant total solute flux at its inlet, with initially zero [concentration](concentration.md) and constant positive [advection](advection.md) speed $U$ and [mass diffusivity](mass-diffusivity.md) $\mathcal D$. A [Laplace transform](laplace-transform.md) in time gives

$$
\widetilde C(x,p)=\frac{2j_0}{p(U+\sqrt{U^2+4\mathcal D p})}\exp\left[\frac{U-\sqrt{U^2+4\mathcal D p}}{2\mathcal D}x\right].
$$

With $\xi=Ux/\mathcal D$, $\vartheta=U^2t/\mathcal D$ and $z_\pm=(\xi\pm\vartheta)/(2\sqrt\vartheta)$, its inverse is

$$
\frac{C(x,t)}{j_0/U}=\frac12\operatorname{erfc}(z_-)+\sqrt{\vartheta/\pi}e^{-z_-^2}-\frac12(1+\xi+\vartheta)e^\xi\operatorname{erfc}(z_+).
$$

The [complementary error function](complementary-error-function.md) describes the smeared front. This is a flux boundary condition, not the [constant-concentration inlet solution](constant-concentration-inlet-solution.md). At large axial [Péclet number](peclet-number.md), both have the leading advancing front $\tfrac12\operatorname{erfc}(z_-)$.

## ↑ Ancestors (7)

1. [Advection-diffusion equation](advection-diffusion-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69/1/solution.md)
