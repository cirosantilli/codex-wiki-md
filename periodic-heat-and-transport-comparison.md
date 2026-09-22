# Periodic heat and transport comparison

↑ **Parent:** [Transport equation](transport-equation-split.md)

Use dimensionless $x$ and $t$, the [periodic domain](periodic-domain.md) $[0,2\pi]$, and the same [initial condition](initial-condition.md)

$$
g(x)=1+\cos x+0.4\cos(3x).
$$

With zero [PDE source term](source-term-in-a-partial-differential-equation.md), compare the [heat equation](heat-equation.md) $u_t=u_{xx}$ and the [transport equation](transport-equation-split.md) $u_t+u_x=0$. Their exact solutions are

$$
u_H(x,t)=1+e^{-t}\cos x+0.4e^{-9t}\cos(3x),\qquad u_T(x,t)=1+\cos(x-t)+0.4\cos(3(x-t)).
$$

Each [cosine](cosine.md) satisfies $\partial_x^2\cos(nx)=-n^2\cos(nx)$, so the [heat equation](heat-equation.md) reduces its amplitude according to $A_n'=-n^2A_n$. The [superposition principle](superposition-principle.md) combines the constant and two [Fourier modes](fourier-mode.md). The [transport equation](transport-equation-split.md) shifts the argument of the entire profile. Both formulas meet the [initial condition](initial-condition.md) and matching [periodic boundary conditions](periodic-boundary-conditions.md) exactly.[Stanford Math 220B heat-equation notes, periodic boundary conditions](https://web.stanford.edu/class/math220b/handouts/heateqn.pdf)

At $t=1$, the heat amplitudes are approximately $0.368$ and $0.0000494$: the small ripples disappear much sooner than the broad variation. The [transport equation](transport-equation-split.md) retains amplitudes $1$ and $0.4$, shifting the profile right by one unit with wraparound. Both preserve spatial average $1$, but only the [heat equation](heat-equation.md) approaches the uniform profile. This gives [diffusion](diffusion.md) its usefulness for smoothing uneven [temperatures](temperature-split.md), while the [transport equation](transport-equation-split.md) models a profile carried by a flow. The signed profile can represent a scaled [temperature](temperature-split.md) deviation.

<a id="image-exact-evolution-of-one-periodic-profile-transport-translates-while-diffusion-preferentially-removes-short-wavelengths"></a>
![](pde-transport-vs-diffusion.png)

**[Figure 1](#image-exact-evolution-of-one-periodic-profile-transport-translates-while-diffusion-preferentially-removes-short-wavelengths). Exact evolution of one periodic profile: transport translates while diffusion preferentially removes short wavelengths**.

To restore units, let physical position be $X=\ell x$ and time be $T=\tau t$. For $U_T=D U_{XX}$, the dimensionless coefficient is $D\tau/\ell^2$, with $D$ measured in length squared per time. For $U_T+cU_X=0$, it is $c\tau/\ell$, with $c$ measured in length per time. Both plotted coefficients equal one when $D=\ell^2/\tau$ and $c=\ell/\tau$. Thus the example compares specified models on the same scales, rather than identifying [diffusivity](diffusion-coefficient.md) with [velocity](velocity.md).

## ↑ Ancestors (6)

1. [Transport equation](transport-equation-split.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Partial differential equation](partial-differential-equation-split.md)
- [Transport equation](transport-equation-split.md)
