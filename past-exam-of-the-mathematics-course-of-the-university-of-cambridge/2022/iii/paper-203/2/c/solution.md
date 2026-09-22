<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By conformal invariance, $g_A(B)$ after its quadratic-variation time-change is Brownian motion in $\mathbb H$, started at

$$
g_A(iy)=x_y+i v_y,
\qquad x_y\to0,\quad v_y/y\to1.
$$

Since $E\subset\mathbb R\setminus[-1,1]$ and $A\subset\overline{\mathbb D}$, the boundary correspondence is regular there, and the exit event maps to $g_A(E)$. The [Poisson kernel](../../../../../../poisson-kernel-for-the-upper-half-plane.md) of $\mathbb H$ therefore gives

$$
\mathbb P^{iy}(B_{\tau_A}\in E)
=\int_{g_A(E)}
\frac{v_y}{(u-x_y)^2+v_y^2}\,\frac{du}{\pi}.
$$

For bounded subsets, multiplication by $y$ makes the integrand converge uniformly to $1/\pi$. Approximation by increasing bounded subsets and [monotone convergence](../../../../../../monotone-convergence-theorem.md) then gives

$$
\lim_{y\to\infty}
y\,\mathbb P^{iy}(B_{\tau_A}\in E)
=\frac{\operatorname{Leb}(g_A(E))}{\pi},
$$

with both sides allowed to be infinite.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
