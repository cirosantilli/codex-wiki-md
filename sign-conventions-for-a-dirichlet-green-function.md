# Sign conventions for a Dirichlet Green function

↑ **Parent:** [Dirichlet Green function](dirichlet-green-function.md)

Let $G$ vanish on the boundary of a domain and satisfy $\Delta G(\cdot,y)=\delta_y$. [Green's second identity](green-second-identity.md) gives

$$
u(y)=\int_\Omega G(x,y)\Delta u(x)dx+\int_{\partial\Omega}u(x)\partial_{n_x}G(x,y)dS_x.
$$

Thus the [Poisson kernel](poisson-kernel.md) is $+\partial_nG$ for this convention. If instead $-\Delta K=\delta$, then $K=-G$ and the same kernel is $-\partial_nK$. At the boundary of $x>0$, the outward normal is $-e_x$, so the first convention gives $P=-\partial_xG$. Changing the delta-source sign or replacing the outward derivative by an inward coordinate derivative changes a sign; changing both leaves the physical kernel unchanged.

## ↑ Ancestors (6)

1. [Dirichlet Green function](dirichlet-green-function.md)
2. [Green's function](green-s-function-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2/1/solution.md)
