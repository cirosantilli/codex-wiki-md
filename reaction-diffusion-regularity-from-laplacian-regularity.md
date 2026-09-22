# Reaction-diffusion regularity from Laplacian regularity

↑ **Parent:** [Elliptic regularity](elliptic-regularity.md)

Suppose the mixed [boundary value problem](boundary-value-problem-split.md) $\Delta w=g$, with zero [Dirichlet boundary condition](dirichlet-boundary-condition.md) on a nonempty boundary portion and zero [Neumann boundary condition](neumann-boundary-condition.md) on the remainder, has an $H^2$ solution with $\|w\|_{H^2}\leq C\|g\|_{L^2}$. Assume the domain is connected and that zero [Sobolev trace](trace-operator.md) on the specified portion excludes nonzero constants. Then the same [boundary conditions](boundary-condition.md) for $-\Delta z+z=e$ give $\|z\|_{H^2}\leq2C\|e\|_{L^2}$.

Indeed, the [Lax-Milgram theorem](lax-milgram-theorem.md) first constructs $z$ in the [Sobolev space with a partial Dirichlet condition](sobolev-space-with-a-partial-dirichlet-condition.md); testing with $z$ shows $\|z\|_{H^1}\leq\|e\|_{L^2}$. Apply the assumed [elliptic regularity](elliptic-regularity.md) result to $g=z-e$. Its solution $w$ and $z$ satisfy the same weak Laplace equation, so testing their difference shows $\nabla(w-z)=0$. The [Sobolev function with zero weak gradient](sobolev-function-with-zero-weak-gradient.md) property and zero [Sobolev trace](trace-operator.md) give $w=z$. Finally $\|z-e\|_{L^2}\leq2\|e\|_{L^2}$. This argument supplies the dual regularity needed by the [Aubin–Nitsche duality argument](aubin-nitsche-duality-argument.md) for the equation with a positive reaction term.

## ↑ Ancestors (7)

1. [Elliptic regularity](elliptic-regularity.md)
2. [Elliptic differential operator](elliptic-differential-operator.md)
3. [Distribution theory](distribution-theory-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/2/e/solution.md)
