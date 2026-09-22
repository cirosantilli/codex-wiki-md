<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The substitution separates the uniform equilibrium from the decaying perturbation. Direct [differentiation](../../../../differentiation.md) gives

$$
u_t=e^{-\beta t}(v_t-\beta v),\qquad u_{xx}=e^{-\beta t}v_{xx},\qquad\beta(u-u_0)=\beta e^{-\beta t}v.
$$

Consequently the [reaction-diffusion equation](../../../../reaction-diffusion-system.md) reduces to the [heat equation](../../../../heat-equation.md) $v_t=v_{xx}$. Its data become

$$
\boxed{v(0,t)=e^{\beta t}(u_1-u_0),\quad v(\pi,t)=e^{\beta t}(u_2-u_0),\quad v(x,0)=f(x)-u_0.}
$$

When the three constants coincide, the [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) for $v$ are homogeneous. [Separation of variables](../../../../separation-of-variables.md) gives $X''+n^2X=0$ and $T'=-n^2T$, selecting the [normal modes](../../../../normal-mode.md) $\sin(nx)e^{-n^2t}$ for $n\geq1$. Thus

$$
v(x,t)=\sum_{n=1}^\infty b_n\sin(nx)e^{-n^2t},\qquad b_n=\frac2\pi\int_0^\pi[x(\pi-x)-u_0]\sin(nx)\,dx.
$$

Two [integrations by parts](../../../../integration-by-parts.md) give $\int_0^\pi x(\pi-x)\sin(nx)dx=2[1-(-1)^n]/n^3$, while the constant term uses $\int_0^\pi\sin(nx)dx=[1-(-1)^n]/n$. Therefore the [Fourier sine series](../../../../fourier-sine-series.md) is

$$
\boxed{v(x,t)=\frac4\pi\sum_{\substack{n\geq1\\n\text{ odd}}}\left(\frac2{n^3}-\frac{u_0}n\right)e^{-n^2t}\sin(nx).}
$$

For $u_0\ne2$, its first coefficient is nonzero. Multiplying by $e^{-\beta t}$ and retaining the slowest-decaying mode gives

$$
\boxed{u(x,t)=u_0-\frac4\pi(u_0-2)e^{-(\beta+1)t}\sin x+O(e^{-(\beta+9)t})\quad(t\to\infty).}
$$

The remainder estimate holds uniformly in $x$ for sufficiently large positive time. If $u_0=2$, the fundamental vanishes and the next possible mode has decay rate $\beta+9$, explaining the exclusion.

There is an initial endpoint compatibility issue unless $u_0=0$: the given polynomial profile vanishes at the endpoints, whereas the boundary values equal $u_0$. The series realizes the initial data in [L2 space](../../../../l2-space-is-a-hilbert-space.md) and pointwise in the open interval, imposing the prescribed boundary values for $t>0$. For nonzero $u_0$ it cannot also be continuous at both initial endpoint corners.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
