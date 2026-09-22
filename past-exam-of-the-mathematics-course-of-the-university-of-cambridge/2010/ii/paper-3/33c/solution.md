<h1 id="33c/solution">Solution</h1>

↑ **Parent:** [33C](../33c.md)

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) are $[\widehat x,\widehat p]=i\hbar I$ (in several dimensions $[x_i,p_j]=i\hbar\delta_{ij}I$, with the position-position and momentum-momentum [commutators](../../../../../commutator.md) zero). For Hermitian $x,p$, the [commutator](../../../../../commutator.md) is anti-Hermitian, just as $i\hbar I$ is; there is no conflict with their self-adjointness. The [annihilation operator](../../../../../annihilation-operator.md) and its adjoint obey

$$
[a,a^\dagger]=\frac1{2\hbar}[x+ip,x-ip]=1,\qquad
N=a^\dagger a=\frac{x^2+p^2-\hbar}{2\hbar}.
$$

Thus the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md) [Hamiltonian](../../../../../hamiltonian.md) is $\boxed{H=\hbar(N+1/2)}$. The [commutators](../../../../../commutator.md) $[N,a]=-a$, $[N,a^\dagger]=a^\dagger$ and the normalized [ground state](../../../../../ground-state.md) construct

$$
\boxed{|n\rangle=\frac{(a^\dagger)^n}{\sqrt{n!}}|0\rangle,\quad
E_n=\hbar(n+1/2),\quad
 a|n\rangle=\sqrt n|n-1\rangle,\quad
 a^\dagger|n\rangle=\sqrt{n+1}|n+1\rangle.}
$$

Normalization follows inductively from $aa^\dagger=N+1$. Positivity of $N$ and repeated lowering exclude a noninteger [eigenvalue](../../../../../eigenvalue.md): lowering it until it becomes negative would produce a nonzero vector of negative $N$ [eigenvalue](../../../../../eigenvalue.md). Every eigenstate therefore lowers to the unique [ground state](../../../../../ground-state.md), so these normalized ladder states exhaust the oscillator eigenstates.

For two independent oscillators, the [tensor products](../../../../../tensor-product.md) $|n_1,n_2\rangle$ have $E=\hbar(n_1+n_2+1)$. The level $n=n_1+n_2$ has **degeneracy $n+1$**. In its degenerate subspace the perturbation $\lambda x_1x_2$ reduces to

$$
\frac{\lambda\hbar}{2}(a_1a_2^\dagger+a_1^\dagger a_2),
$$

since terms that raise or lower both numbers leave the subspace. For $n=0$ its matrix is zero. For $n=1$, in $|1,0\rangle,|0,1\rangle$, it is $(\lambda\hbar/2)\begin{pmatrix}0&1\\1&0\end{pmatrix}$. For $n=2$, in $|2,0\rangle,|1,1\rangle,|0,2\rangle$, it is $(\lambda\hbar/2)\begin{pmatrix}0&\sqrt2&0\\\sqrt2&0&\sqrt2\\0&\sqrt2&0\end{pmatrix}$. Their [eigenvalues](../../../../../eigenvalue.md) give

$$
\boxed{\begin{array}{c|c}
 n&\text{energies through first order}\\\hline
0&\hbar+O(\lambda^2)\\
1&2\hbar\pm\lambda\hbar/2+O(\lambda^2)\\
2&3\hbar-\lambda\hbar,\ 3\hbar,\ 3\hbar+\lambda\hbar\quad+O(\lambda^2).
\end{array}}
$$

The $n=1$ states are the symmetric and antisymmetric combinations. At $n=2$, the shifted states are $(|2,0\rangle\pm\sqrt2|1,1\rangle+|0,2\rangle)/2$, and the zero-shift state is $(|2,0\rangle-|0,2\rangle)/\sqrt2$.

## ↑ Ancestors (10)

1. [33C](../33c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
