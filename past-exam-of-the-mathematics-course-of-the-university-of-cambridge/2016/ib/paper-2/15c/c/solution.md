<h1 id="15c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With unit constant bending coefficients and unit length, the quadratic [elastic energy](../../../../../../elastic-energy.md) is

$$
E=\frac12\int_0^1\left(y''^2+z''^2-F(y'^2+z'^2)\right)\,dx.
$$

To find the first loss of positivity, put $v=y'$. The clamped conditions give $v(0)=v(1)=0$ and $\int_0^1v\,dx=0$. Extend $v$ periodically with period one. The sharp [periodic Wirtinger inequality](../../../../../../periodic-wirtinger-inequality.md) gives $\int_0^1v'^2\,dx\ge4\pi^2\int_0^1v^2\,dx$. For completeness, expand the mean-zero periodic $v$ in its [Fourier series](../../../../../../fourier-series-split.md) $\sum_{n\ge1}(a_n\cos2\pi nx+b_n\sin2\pi nx)$. [Parseval identity](../../../../../../parseval-identity.md) gives

$$
\int_0^1v^2\,dx=\frac12\sum_{n\ge1}(a_n^2+b_n^2),\qquad
\int_0^1v'^2\,dx=\frac12\sum_{n\ge1}(2\pi n)^2(a_n^2+b_n^2),
$$

which proves the inequality and its equality condition. The same holds for $z'$. Consequently

$$
E\ge\frac{4\pi^2-F}{2}\int_0^1(y'^2+z'^2)\,dx.
$$

For $F<4\pi^2$, the straight filament is the unique minimum. Equality in the [periodic Wirtinger inequality](../../../../../../periodic-wirtinger-inequality.md) has $v=a\cos2\pi x+b\sin2\pi x$; the endpoint value $v(0)=0$ eliminates $a$. Integration and the position boundary conditions therefore give **the first buckling load and modes**:

$$
\boxed{F_c=4\pi^2,\qquad y=\alpha(1-\cos2\pi x),\quad z=\beta(1-\cos2\pi x).}
$$

At this load every such pair has zero quadratic [elastic energy](../../../../../../elastic-energy.md) and solves the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md). For $F>F_c$ these modes give negative energy, signaling instability of the straight configuration. The quadratic small-slope model does not select a finite post-buckling amplitude; nonlinear terms would be needed for that. This is [Euler buckling of an elastic filament](../../../../../../euler-buckling-of-an-elastic-filament.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15C](../../15c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
