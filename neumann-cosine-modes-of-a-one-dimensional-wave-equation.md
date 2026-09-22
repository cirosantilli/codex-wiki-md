# Neumann cosine modes of a one-dimensional wave equation

↑ **Parent:** [Wave equation](wave-equation-split.md)

For the [wave equation](wave-equation-split.md) $\psi_{tt}=c^2\psi_{xx}$ on $0<x<L$, impose homogeneous [Neumann boundary conditions](neumann-boundary-condition.md) $\psi_x(0,t)=\psi_x(L,t)=0$, where $c,L>0$. [Separation of variables](separation-of-variables.md) gives $X''+\lambda X=0$ and $T''+c^2\lambda T=0$. [Integration by parts](integration-by-parts.md) gives $\int_0^L(X')^2dx=\lambda\int_0^LX^2dx$, so every nontrivial spatial [eigenfunction](eigenfunction.md) has $\lambda\geq0$.

For $\lambda=0$, $X$ is constant and $T=A_0+B_0t$. For $\lambda>0$, the boundary conditions select $\lambda_n=(n\pi/L)^2$ and $X_n=\cos(n\pi x/L)$. The [superposition principle](superposition-principle.md) gives the displayed expansion when the initial data have sufficient regularity. The constant [zero mode](zero-mode.md) must be retained: homogeneous [Neumann boundary conditions](neumann-boundary-condition.md) do not force the spatial average of the displacement to vanish.

With zero initial [velocity](velocity.md), all $B_n$ vanish, including $B_0$. Initial displacement $a+b\cos(n\pi x/L)$ then evolves as $a+b\cos(cn\pi t/L)\cos(n\pi x/L)$, a [standing wave](standing-wave.md) above a constant offset.

## ↑ Ancestors (6)

1. [Wave equation](wave-equation-split.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
