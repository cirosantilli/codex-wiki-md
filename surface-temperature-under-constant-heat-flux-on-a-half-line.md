# Surface temperature under constant heat flux on a half-line

↑ **Parent:** [Heat equation](heat-equation.md)

For [thermal diffusivity](thermal-diffusivity.md) $\kappa>0$ and [thermal conductivity](thermal-conductivity.md) $k>0$, a semi-infinite conductor satisfies $u_t=\kappa u_{xx}$ for $x>0$. Take zero initial [temperature](temperature-split.md) and constant incoming [heat flux](heat-flux-density.md) $-ku_x(0,t)=Q$. Select the physical solution by boundedness at spatial infinity together with sufficient growth control for the time [Laplace transform](laplace-transform.md).

Writing the time transform as $U$ gives $U_{xx}=(p/\kappa)U$. The decaying branch is $U=A(p)e^{-x\sqrt{p/\kappa}}$, where $\operatorname{Re}\sqrt p>0$. The transformed flux condition gives $A=Q\sqrt\kappa/(kp^{3/2})$. Since $\mathcal L[2\sqrt t]=\sqrt\pi p^{-3/2}$, inversion gives the displayed surface [temperature](temperature-split.md). More generally the full profile is

$$
u(x,t)=\frac Qk\left[2\sqrt{\frac{\kappa t}{\pi}}e^{-x^2/(4\kappa t)}-x\operatorname{erfc}\!\left(\frac{x}{2\sqrt{\kappa t}}\right)\right].
$$

Differentiation verifies the [heat equation](heat-equation.md) and the applied flux; for every $x>0$ it tends to zero at initial time and decays at spatial infinity. Its surface [temperature](temperature-split.md) grows as $\sqrt t$, because the depth significantly heated by [diffusion](diffusion.md) has the same scale.

## ↑ Ancestors (7)

1. [Heat equation](heat-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2004/9/solution.md)
