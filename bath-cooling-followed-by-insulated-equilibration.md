# Bath cooling followed by insulated equilibration

↑ **Parent:** [Heat equation](heat-equation.md)

Let a homogeneous plate $0<x<L$ begin at uniform [temperature](temperature-split.md) $T_0$, cool with zero-temperature [Dirichlet boundary conditions](dirichlet-boundary-condition.md) until time $t_b$, then switch to insulated [Neumann boundary conditions](neumann-boundary-condition.md). For [thermal diffusivity](thermal-diffusivity.md) $\kappa>0$, the [Fourier sine series](fourier-sine-series.md) during cooling is $T=(4T_0/\pi)\sum_{n\geq1,\ n\text{ odd}}\sin(n\pi x/L)e^{-\kappa(n\pi/L)^2t}/n$. Integrating the insulated [heat equation](heat-equation.md) shows that its [integral average](integral-average.md) is conserved. All nonconstant [Fourier cosine series](fourier-cosine-series.md) modes then decay, proving that the final uniform [temperature](temperature-split.md) is $T_\infty=(8T_0/\pi^2)\sum_{n\geq1,\ n\text{ odd}}e^{-\kappa(n\pi/L)^2t_b}/n^2$. Its limits are $T_0$ at zero bath time and zero at infinite bath time. Instantaneous changes of boundary condition can create initial-boundary corner incompatibilities without invalidating the positive-time solution.

## ↑ Ancestors (7)

1. [Heat equation](heat-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford/2023/paper-1/10/e/solution.md)
