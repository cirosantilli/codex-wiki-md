# Heat equation on a rectangle with two insulated sides

↑ **Parent:** [Heat equation](heat-equation.md)

On $0<x<a$, $0<y<b$, impose zero [Dirichlet boundary conditions](dirichlet-boundary-condition.md) at $x=0,a$ and zero [Neumann boundary conditions](neumann-boundary-condition.md) at $y=0,b$. [Separation of variables](separation-of-variables.md) for $T_t=\lambda\Delta T$ gives the displayed sine-cosine expansion. The zero cosine mode must be included: its norm is $b$, whereas the positive cosine modes have norm $b/2$. Thus $A_{n0}=2(ab)^{-1}\int\!\int T_0\sin(n\pi x/a)$ and $A_{nm}=4(ab)^{-1}\int\!\int T_0\sin(n\pi x/a)\cos(m\pi y/b)$ for $m\geq1$. Expanding $x(a-x)$ gives sine coefficient $4a^2[1-(-1)^n]/(n^3\pi^3)$. Initial data $x(a-x)\sin^2(2\pi y/b)$ therefore involve only $m=0,4$ and odd $n$. Their leading long-time mode is $4a^2\sin(\pi x/a)e^{-\lambda\pi^2t/a^2}/\pi^3$.

## ↑ Ancestors (7)

1. [Heat equation](heat-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/2/a/solution.md)
