<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p$ be the collocation polynomial of degree at most $s$ over one step, with $p(t_n)=y_n$, and let $Y_i=p(t_n+c_ih)$. Its derivative, of degree at most $s-1$, is fixed by its values at the distinct nodes. [Lagrange interpolation](../../../../../../lagrange-polynomial.md) therefore gives

$$
p'(t_n+h\tau)=\sum_{j=1}^s\ell_j(\tau)f(t_n+c_jh,Y_j).
$$

Integrating from zero to $\tau$ yields

$$
p(t_n+h\tau)=y_n+h\sum_{j=1}^s
\left(\int_0^\tau\ell_j(v)\,dv\right)f(t_n+c_jh,Y_j).
$$

At $\tau=c_i$ this gives the stage equations of an [implicit Runge-Kutta method](../../../../../../implicit-runge-kutta-method.md); at $\tau=1$ it gives the update. Consequently

$$
\boxed{a_{ij}=\int_0^{c_i}\ell_j(v)\,dv,\qquad
b_j=\int_0^1\ell_j(v)\,dv.}
$$

Conversely, stages satisfying these equations define the integrated polynomial displayed above. It takes the stage values at the nodes and has the required derivative there, so it solves the collocation equations. This proves equivalence for every common solution branch, not merely equality on the scalar test equation. Also $\sum_ja_{ij}=c_i$, since the Lagrange polynomials sum to one. Stage existence or uniqueness requires the usual implicit-solvability assumptions; for a Lipschitz vector field a sufficiently small step gives a contraction. This is the [collocation Runge-Kutta method](../../../../../../collocation-runge-kutta-method.md) construction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
