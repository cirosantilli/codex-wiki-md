<h1 id="12b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [spherically symmetric function](../../../../../../spherically-symmetric-function.md) $\Phi(r)$, the [Laplacian in spherical coordinates](../../../../../../laplacian-in-spherical-coordinates.md) is

$$
\nabla^2\Phi=\frac1{r^2}\frac{d}{dr}(r^2\Phi').
$$

Integrating from zero to $r$ and using regularity at the origin gives

$$
\boxed{4\pi r^2\Phi'(r)=4\pi\int_0^rs^2\rho(s)\,ds}.
$$

For the stated density, integration and the boundary condition $\Phi(a)=0$ give

$$
\boxed{
\Phi(r)=
\begin{cases}
\displaystyle \rho_0\left(\frac{r^2}{6}-\frac{b^2}{2}+\frac{b^3}{3a}\right),&0\leq r\leq b,\\[6pt]
\displaystyle \frac{\rho_0b^3}{3}\left(\frac1a-\frac1r\right),&b<r\leq a.
\end{cases}}
$$

The two pieces and their first derivatives agree at $r=b$. If another solution existed, its difference from $\Phi$ would be [harmonic](../../../../../../harmonic-function.md) with zero boundary data, so part (a) proves [Uniqueness of the Dirichlet problem](../../../../../../uniqueness-of-the-dirichlet-problem.md).

On the shell $U(b,a)$, normalize the outer radial part to obtain the harmonic function

$$
v(r)=\frac{b(a-r)}{(a-b)r},
\qquad v(b)=1,\quad v(a)=0.
$$

By the [Dirichlet principle](../../../../../../dirichlet-principle.md), this function minimizes the energy among all $w$ with the same boundary values. Since

$$
v'(r)=-\frac{ab}{(a-b)r^2},
$$

its energy is

$$
4\pi\int_b^a r^2|v'(r)|^2dr
=\frac{4\pi a^2b^2}{(a-b)^2}\left(\frac1b-\frac1a\right)
=\frac{4\pi ab}{a-b}.
$$

Therefore

$$
\boxed{\int_{U(b,a)}|\nabla w|^2dV\geq\frac{4\pi ab}{a-b}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12B](../../12b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
