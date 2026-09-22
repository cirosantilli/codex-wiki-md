# No positive-Courant cancellation for backward Euler diffusion

↑ **Parent:** [Backward Euler diffusion scheme](backward-euler-diffusion-scheme.md)

For a smooth solution of the [heat equation](heat-equation.md), backward Euler with the centered second difference has residual divided by $k$ equal to $-(k/2+d^2/12)u_{xxxx}+O(k^2+kd^2+d^4)$. Both leading terms have the same sign. Under [parabolic mesh refinement](parabolic-mesh-refinement.md) their coefficient is $-d^2(r/2+1/12)$, which cannot vanish for a positive [diffusion Courant number](diffusion-courant-number.md). Consistency of an update $U^{n+1}-U^n=\alpha(r)\delta^2U^{n+1}$ forces $\alpha(r)=r$ for every fixed positive $r$.

## ↑ Ancestors (9)

1. [Backward Euler diffusion scheme](backward-euler-diffusion-scheme.md)
2. [von Neumann stability analysis](von-neumann-stability-analysis.md)
3. [Finite difference method](finite-difference-method.md)
4. [Finite difference](finite-difference-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
