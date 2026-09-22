<h1 id="32b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume periodic boundary conditions or sufficient decay so that integrations by parts have no boundary terms. Use the Hamiltonian operator $\mathcal J=\partial_x$ and the functional

$$
\boxed{H[u]=\int\left[\frac{u^{n+2}}{(n+1)(n+2)}+\frac{(-1)^k}{2}(\partial_x^ku)^2\right]dx.}
$$

For a variation $u+\varepsilon v$, integrate the second term by parts $k$ times. The two factors $(-1)^k$ cancel, giving

$$
\frac{\delta H}{\delta u}=\frac{u^{n+1}}{n+1}+\partial_x^{2k}u.
$$

Thus $\boxed{u_t=\mathcal J\,\delta H/\delta u}$ is exactly the equation, including $k=0$ and $n=0$. The bracket $\{F,G\}=\int(\delta F/\delta u)\partial_x(\delta G/\delta u)dx$ is antisymmetric by integration by parts. Since this differential operator has coefficients independent of $u$, its associated constant Poisson bracket satisfies the Jacobi identity. This supplies a genuine [Hamiltonian field equation](../../../../../../hamiltonian-field-equation.md), not just a conserved scalar functional.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [32B](../../32b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
