<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a nonzero separated solution $u=X(x)T(t)$ of the [reaction-diffusion equation](../../../../../reaction-diffusion-system.md), substitution and division by $XT$ gives

$$
\frac{T'}T+1=\frac{X''}X.
$$

The two sides depend on different variables, so both equal a separation constant. The homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) select a negative spatial constant, written $-k^2$:

$$
X''+k^2X=0,\qquad T'+(1+k^2)T=0.
$$

For $k>0$, $X=A\sin kx+B\cos kx$. The boundary value at zero makes $B=0$; the boundary value at $L$ then requires $kL=n\pi$, with $n=1,2,\ldots$. A zero spatial constant gives only a linear [function](../../../../../function-split.md) vanishing at both endpoints, hence the zero [function](../../../../../function-split.md); a positive spatial constant similarly gives no nonzero admissible hyperbolic solution. Therefore

$$
\boxed{X_n(x)=A_n\sin\frac{n\pi x}{L},\qquad
T_n(t)=B_n\exp\left[-\left(1+\frac{n^2\pi^2}{L^2}\right)t\right]}.
$$

By [superposition](../../../../../superposition-principle.md), the [general solution](../../../../../general-solution.md) with the stated boundary conditions is

$$
\boxed{u(x,t)=\sum_{n=1}^\infty c_n\sin\frac{n\pi x}{L}
\exp\left[-\left(1+\frac{n^2\pi^2}{L^2}\right)t\right]}.
$$

The coefficients are fixed only if initial data are supplied: for $u(x,0)=f(x)$, they are the [Fourier sine series](../../../../../fourier-sine-series.md) coefficients $c_n=(2/L)\int_0^L f(x)\sin(n\pi x/L)\,dx$. Here they remain arbitrary subject to convergence. Every mode has the ordinary diffusive decay rate plus the additional reaction decay rate one.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
