<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose both circular ends of the cylinder to be electric, or rough, boundaries. In the convention of part 1, retain plaquette generators

$$
B_p=\prod_{e\in\partial p}Z_e
$$

with their boundary truncations, and use star generators

$$
A_v=\prod_{e\ni v}X_e
$$

only at vertices not lying on an electric boundary. Omitting the endpoint star checks allows a $Z$ string to terminate at either boundary, which is precisely [anyon condensation at a boundary](../../../../../../anyon-condensation-at-a-boundary.md) for $e$.

Relative homology now has one nontrivial class represented by a primal $Z$ path $\gamma$ joining the two boundaries. The dual absolute homology has one class represented by an $X$ loop $\widetilde\gamma$ around the cylinder. Their strings intersect once and anticommute, so they form one logical pair $\bar Z,\bar X$. Every other closed or boundary-ending string is a product of stabilizers, so the code has exactly one logical qubit.

In the [Random-bond Ising model](../../../../../../random-bond-ising-model.md) mapping, there is no Ising spin for an omitted boundary star. An edge $e$ joining an interior vertex $v$ to an electric boundary is toggled by only $A_v$, so its bond factor $\eta_e\sigma_v\sigma_{v'}$ is replaced by the boundary-field factor $\eta_e\sigma_v$. Equivalently, attach exterior spins fixed to $+1$ and retain the same bond formula. Edges wholly on a boundary contribute fixed constants. The bulk Hamiltonian is therefore supplemented by

$$
H_{\partial}=-J\sum_{e=(v,\partial)}\eta_e(s,q)\sigma_v,
$$

with the signs still determined by $E_s\bar X^q$. This is the required boundary modification.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
