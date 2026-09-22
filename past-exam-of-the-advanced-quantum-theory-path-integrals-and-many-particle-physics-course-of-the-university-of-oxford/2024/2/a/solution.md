<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V=L^3$ be the box [volume](../../../../volume.md). The [number operator](../../../../number-operator.md) is the sum of the [occupation numbers](../../../../occupation-number.md) of all [momentum eigenstates](../../../../momentum-eigenstate.md), including the zero mode:

$$
\boxed{\hat N=\int_V d^3r\,\psi^\dagger(\mathbf r)\psi(\mathbf r)
=\sum_{\mathbf k}\psi_{\mathbf k}^\dagger\psi_{\mathbf k}.}
$$

In the [Fourier series](../../../../fourier-series-split.md) for the [contact interaction](../../../../contact-interaction-quantum-mechanics.md), the two [creation operators](../../../../creation-operator.md) supply phase $e^{-i(\mathbf k_1+\mathbf k_2)\cdot\mathbf r}$ and the two [annihilation operators](../../../../annihilation-operator.md) supply $e^{i(\mathbf k_3+\mathbf k_4)\cdot\mathbf r}$. [Fourier orthogonality](../../../../fourier-orthogonality.md) with [periodic boundary conditions](../../../../periodic-boundary-conditions.md) gives

$$
\int_V d^3r\,e^{i(\mathbf k_3+\mathbf k_4-\mathbf k_1-\mathbf k_2)\cdot\mathbf r}
=V\delta_{\mathbf k_1+\mathbf k_2,\,\mathbf k_3+\mathbf k_4}.
$$

The four normalization factors together contribute $V^{-2}$, leaving the [momentum-space contact-interaction Hamiltonian](../../../../momentum-space-contact-interaction-hamiltonian.md)

$$
\boxed{H_{\rm int}=\frac{u}{2V}
\sum_{\mathbf k_1,\mathbf k_2,\mathbf k_3,\mathbf k_4}
\delta_{\mathbf k_1+\mathbf k_2,\,\mathbf k_3+\mathbf k_4}
\psi_{\mathbf k_1}^\dagger\psi_{\mathbf k_2}^\dagger
\psi_{\mathbf k_3}\psi_{\mathbf k_4}.}
$$

The [Kronecker delta](../../../../kronecker-delta.md) enforces [momentum conservation](../../../../momentum-conservation.md). An equivalent expression that resolves the momentum transfer is

$$
H_{\rm int}=\frac{u}{2V}\sum_{\mathbf k,\mathbf p,\mathbf q}
\psi_{\mathbf k+\mathbf q}^\dagger\psi_{\mathbf p-\mathbf q}^\dagger
\psi_{\mathbf p}\psi_{\mathbf k}.
$$

Both are already in [normal ordering](../../../../normal-ordering.md); no extra [commutator](../../../../commutator.md) constant is introduced.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
