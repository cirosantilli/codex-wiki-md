# Probabilistic representation of the heat equation with time-dependent Dirichlet data

↑ **Parent:** [Heat equation](heat-equation.md)

For $u_t=\frac12u_{xx}$ on $(0,1)$ with initial data $g$ and time-dependent [Dirichlet boundary conditions](dirichlet-boundary-condition.md) $f_1,f_2$, stop [Brownian motion](brownian-motion-split.md) at its first hit of $0$ or $1$. Applying [Itô formula](ito-s-lemma.md) to $u(t-s,B_s)$ yields

$$
u(t,x)=\mathbb E_x\!\left[g(B_t)\mathbf1_{\{t<\tau_0\wedge\tau_1\}}+f_1(t-\tau_0)\mathbf1_{\{\tau_0<t\wedge\tau_1\}}+f_2(t-\tau_1)\mathbf1_{\{\tau_1<t\wedge\tau_0\}}\right].
$$

## ↑ Ancestors (7)

1. [Heat equation](heat-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202/6/c/solution.md)
