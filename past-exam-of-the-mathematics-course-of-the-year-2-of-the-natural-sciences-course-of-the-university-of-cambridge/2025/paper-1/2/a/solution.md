<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [separation of variables](../../../../../separation-of-variables.md), take $n=T(t)X(x)Y(y)Z(z)$ and divide the [reaction-diffusion equation](../../../../../reaction-diffusion-system.md) by this product wherever it is nonzero:

$$
\frac{T'}{\mu T}-\frac\gamma\mu=\frac{X''}{X}+\frac{Y''}{Y}+\frac{Z''}{Z}.
$$

Each spatial term depends on a different variable and must be constant. Write $X''=-k_x^2X$ and similarly for the other two factors. The [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) give $X(0)=X(L)=0$. A zero separation constant permits only a linear function and hence the zero solution; a positive value of $X''/X$ likewise permits no nonzero function vanishing at both endpoints. The nontrivial choices are therefore

$$
\boxed{X_p(x)=\sin\frac{p\pi x}{L},\quad Y_q(y)=\sin\frac{q\pi y}{L},\quad Z_r(z)=\sin\frac{r\pi z}{L},\qquad p,q,r=1,2,\ldots.}
$$

The temporal [ordinary differential equation](../../../../../ordinary-differential-equation.md) is

$$
T'_{p,q,r}=\left[\gamma-\frac{\mu\pi^2}{L^2}(p^2+q^2+r^2)\right]T_{p,q,r},
$$

so, absorbing its constant multiplier into $a_{p,q,r}$,

$$
\boxed{T_{p,q,r}(t)=\exp\left\{\left[\gamma-\frac{\mu\pi^2}{L^2}(p^2+q^2+r^2)\right]t\right\}.}
$$

The [superposition principle](../../../../../superposition-principle.md) and completeness of the [Fourier sine series](../../../../../fourier-sine-series.md) give the stated threefold expansion with these factors. For an initial density $n_0$, [orthogonality](../../../../../orthogonal-vectors.md) also determines the constants:

$$
a_{p,q,r}=\frac8{L^3}\int_0^L\int_0^L\int_0^L n_0(x,y,z)\sin\frac{p\pi x}{L}\sin\frac{q\pi y}{L}\sin\frac{r\pi z}{L}\,dx\,dy\,dz.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
