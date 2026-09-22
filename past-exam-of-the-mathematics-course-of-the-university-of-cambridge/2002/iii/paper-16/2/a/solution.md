<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the spatial supremum-norm convention, a normalized [Hamiltonian function](../../../../../../hamiltonian-function.md) gives the path length

$$
\ell_\infty(H)=\int_0^1\|H_t\|_\infty\,dt,\qquad \|H_t\|_\infty=\sup_{x\in M}|H_t(x)|.
$$

On an open manifold use compactly supported Hamiltonians; on a closed manifold use zero-mean Hamiltonians, which fixes their additive time-dependent constants. The [Hofer metric from the spatial supremum norm](../../../../../../hofer-metric-from-the-spatial-supremum-norm.md) is

$$
\boxed{\rho_\infty(\phi,\psi)=\inf_{\phi_H^1=\phi^{-1}\psi}\ell_\infty(H)}.
$$

Equivalently one minimizes this length over Hamiltonian paths joining the two maps. Inversion and conjugation preserve the generator's supremum norm, so the distance is symmetric and bi-invariant; concatenation gives the triangle inequality. Its nondegeneracy is the geometric assertion proved in Question 3, not a consequence of these formal properties alone.

Another common convention for [Hofer's metric](../../../../../../hofer-metric.md) uses the oscillation length $\ell_{\mathrm{osc}}(H)=\int_0^1(\max H_t-\min H_t)\,dt$, giving a distance $d_H$. Normalized or compactly supported Hamiltonians have values straddling zero, so

$$
\|H_t\|_\infty\leq\operatorname{osc}H_t\leq2\|H_t\|_\infty,\qquad \rho_\infty\leq d_H\leq2\rho_\infty.
$$

Thus these conventions give equivalent distances, and agree on whether an energy vanishes. We keep the same chosen convention in every energy estimate.

The [Hamiltonian displacement energy](../../../../../../displacement-energy-symplectic-geometry.md) of a subset $A$ is

$$
\boxed{e(A)=\inf\{\rho_\infty(\mathrm{id},\phi):\phi\in\operatorname{Ham}_c(M,\omega),\ \phi(A)\cap A=\varnothing\}}.
$$

The infimum is $+\infty$ if there is no displacing map. In the oscillation convention replace $\rho_\infty$ by $d_H$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
