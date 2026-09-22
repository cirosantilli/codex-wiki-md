# Forward Euler stability for centered advection-diffusion

↑ **Parent:** [von Neumann stability analysis](von-neumann-stability-analysis.md)

For $u_t=u_{xx}+\alpha u_x$ on the whole line, apply centered differences in space and the [Forward Euler method](euler-method.md) in time. With $r=\Delta t/(\Delta x)^2$ and $c=\alpha\Delta t/\Delta x$, the amplification factor is

$$
G(\theta)=1-4r\sin^2(\theta/2)+ic\sin\theta.
$$

Putting $s=\sin^2(\theta/2)$ gives

$$
|G|^2-1=4s\{c^2-2r+(4r^2-c^2)s\}.
$$

For $\Delta t>0$, the affine expression in braces is nonpositive on $[0,1]$ exactly when $r\leq1/2$ and $c^2\leq2r$. Hence [von Neumann stability analysis](von-neumann-stability-analysis.md) gives

$$
\Delta t\leq\frac{(\Delta x)^2}{2},
\qquad\alpha^2\Delta t\leq2.
$$

These conditions are weaker than requiring every stencil weight to be nonnegative; [stability](stability-of-a-numerical-method.md) in the discrete [L2 norm](l2-norm.md) need not imply monotonicity.

## ↑ Ancestors (8)

1. [von Neumann stability analysis](von-neumann-stability-analysis.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/3/b/solution.md)
