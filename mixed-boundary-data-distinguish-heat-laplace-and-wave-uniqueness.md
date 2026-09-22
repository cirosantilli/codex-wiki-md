# Mixed boundary data distinguish heat, Laplace and wave uniqueness

↑ **Parent:** [Initial and boundary data for evolution equations](initial-and-boundary-data-for-evolution-equations.md)

On the unit square, these data determine only the zero solution of the [heat equation](heat-equation.md) $u_y=u_{xx}$. The squared $L^2$ [norm](norm.md) decreases because its derivative is $-2\int u_x^2\,dx$, and its initial value is zero. For [Laplace's equation](laplace-equation.md), $\sin(\pi x/2)\sinh(\pi y/2)$ is a nonzero solution with the same three data; adding zero [Dirichlet data](dirichlet-boundary-data.md) on the top edge restores [uniqueness](uniqueness.md) by [Green's first identity](green-s-first-identity.md). For the [wave equation](wave-equation-split.md) $u_{yy}=u_{xx}$, $\sin(\pi x/2)\sin(\pi y/2)$ is a counterexample; the missing datum is [initial velocity](initial-velocity.md). Adding $u_y(x,0)=0$ restores [uniqueness](uniqueness.md) by conservation of $\frac12\int(u_x^2+u_y^2)\,dx$. Thus the type of equation determines what information is needed on an unprescribed edge.

## ↑ Ancestors (6)

1. [Initial and boundary data for evolution equations](initial-and-boundary-data-for-evolution-equations.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
