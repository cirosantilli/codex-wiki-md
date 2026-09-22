<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For positions $\mathbf r_1,\mathbf r_2$, the two-particle [Schrödinger equation](../../../../../schrodinger-equation.md) is

$$
\boxed{
i\hbar\frac{\partial\Psi}{\partial t}
=\left[-\frac{\hbar^2}{2m}(\nabla_1^2+\nabla_2^2)
-\frac{Gm^2}{|\mathbf r_1-\mathbf r_2|}\right]\Psi}.
$$

Neglecting packet spreading and writing $|a\rangle_i$ for $\psi_{ai}$, branchwise evolution gives

$$
|\Psi(t)\rangle\simeq\frac13\sum_{a,b=0}^2
\exp\left(\frac{iGm^2t}{\hbar d_{ab}}\right)
|a\rangle_1|b\rangle_2,
$$

up to local kinetic phases. This branch-dependent [Newtonian gravitational potential energy](../../../../../newtonian-gravitational-potential-energy.md) produces [gravitationally induced entanglement](../../../../../gravitationally-induced-entanglement.md).

Under the stated distance approximation, only the three branches $a=b$ acquire an appreciable common phase

$$
\phi=\frac{Gm^2t}{\hbar d}.
$$

The coefficient matrix is

$$
C=\frac13[J+(e^{i\phi}-1)I],
$$

where $J$ is the $3\times3$ all-ones matrix. The [reduced density matrix](../../../../../reduced-density-matrix.md) is

$$
\rho_1=CC^\dagger
=\frac19\left[(1+2\cos\phi)J
+2(1-\cos\phi)I\right].
$$

It equals $I/3$ when $\cos\phi=-1/2$, so the first maximally entangled state occurs at $\phi=2\pi/3$. Therefore

$$
\boxed{t_{\rm ent}
=\frac{2\pi\hbar d}{3Gm^2}
=\frac{hd}{3Gm^2}}
\simeq6.6\ {\rm s}.
$$

The state does not remain entangled for every $t>0$. Whenever $\phi=2\pi k$, all branch phases again agree and the state returns to its initial [product state](../../../../../product-state.md). The revival period is

$$
\boxed{T=\frac{2\pi\hbar d}{Gm^2}
=\frac{hd}{Gm^2}\simeq19.7\ {\rm s}}.
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 325](../../paper-325-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
