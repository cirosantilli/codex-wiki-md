<h1 id="11b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $q=-\kappa\nabla T$ and $\nabla\cdot q=H$, the divergence theorem gives

$$
\oint_Sq\cdot dS=\int_VH\,dV.
$$

Spherical symmetry gives $(r^2\kappa T')'=-r^2H$. Regularity at zero and decay at infinity yield

$$
T(r)=\begin{cases}
\displaystyle \frac{H_0}{3(\alpha+1)}+\frac{H_0}{3(2-\alpha)}(1-r^{2-\alpha}),&r\leq1,\\[6pt]
\displaystyle \frac{H_0}{3(\alpha+1)}r^{-\alpha-1},&r>1.
\end{cases}
$$

For $\alpha\leq-1$, the exterior solution cannot tend to zero: it is logarithmic at $-1$ and grows below it.

On the exterior domain, the energy-minimizing solution with boundary value one is $\phi=r^{-\alpha-1}$. Applying the [Dirichlet principle](../../../../../../dirichlet-principle.md) to any admissible $w$ gives

$$
\boxed{\int_1^\infty r^{\alpha+2}(w')^2dr
\geq\int_1^\infty r^{\alpha+2}(\phi')^2dr
=\alpha+1.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11B](../../11b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
