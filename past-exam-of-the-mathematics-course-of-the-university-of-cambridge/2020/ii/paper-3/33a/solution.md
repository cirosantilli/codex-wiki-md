<h1 id="33a/solution">Solution</h1>

↑ **Parent:** [33A](../33a.md)

A [boson](../../../../../boson.md) is an identical particle whose total [multiparticle quantum state](../../../../../multiparticle-quantum-state.md) is symmetric under exchange of any two particles, whereas a [fermion](../../../../../fermion.md) has a total state that is antisymmetric under every exchange. The [Spin-statistics theorem](../../../../../spin-statistics-theorem.md) associates integer spin with bosons and half-integer spin with fermions.

For three distinguishable spin-one particles, the spin [Hilbert space](../../../../../hilbert-space-split.md) has dimension

$$
3^3=27.
$$

Let

$$
\mathbf S=\mathbf S_1+\mathbf S_2+\mathbf S_3
$$

be the [total angular momentum operator](../../../../../total-angular-momentum-operator.md). Since each particle has

$$
\mathbf S_i^2=1(1+1)\hbar^2=2\hbar^2,
$$

we have

$$
\mathbf S^2=6\hbar^2
+2(\mathbf S_1\mathbin\cdot\mathbf S_2
+\mathbf S_2\mathbin\cdot\mathbf S_3
+\mathbf S_3\mathbin\cdot\mathbf S_1).
$$

The [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) is consequently

$$
H=\frac\lambda{\hbar^2}(\mathbf S^2-6\hbar^2).
$$

On the [total-spin sector](../../../../../total-spin-sector.md) with quantum number $J$, its [energy eigenvalue](../../../../../energy-eigenvalue.md) is

$$
E_J=\lambda[J(J+1)-6].
$$

The [Clebsch-Gordan decomposition](../../../../../clebsch-gordan-decomposition.md) may be performed by first coupling particles $1$ and $2$. Their intermediate spin is $j_{12}=0,1,2$, and coupling the third spin gives

$$
\begin{array}{c|c}
j_{12}&J\\ \hline
0&1\\
1&0,1,2\\
2&1,2,3.
\end{array}
$$

Thus the [three spin-one angular-momentum decomposition](../../../../../three-spin-one-angular-momentum-decomposition.md) contains total spin $J=0,1,2,3$ with multiplicities $1,3,2,1$. Multiplying each multiplicity by the multiplet dimension $2J+1$ gives

$$
\begin{array}{c|c|c}
J&E_J&\text{degeneracy}\\ \hline
0&-6\lambda&1\\
1&-4\lambda&9\\
2&0&10\\
3&6\lambda&7.
\end{array}
$$

The degeneracies sum to $27$, as required.

When the particles are indistinguishable, their integer spin makes them bosons. Their common spatial wavefunction is symmetric, so their spin wavefunction must also lie in the [symmetric three-spin-one subspace](../../../../../symmetric-three-spin-one-subspace.md). Its decomposition is

$$
\operatorname{Sym}^3(1)=3\oplus1.
$$

Hence only the $J=3$ and $J=1$ levels remain, now with one copy of each multiplet:

$$
\boxed{
E=-4\lambda\text{ has degeneracy }3,
\qquad
E=6\lambda\text{ has degeneracy }7.}
$$

## ↑ Ancestors (10)

1. [33A](../33a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
