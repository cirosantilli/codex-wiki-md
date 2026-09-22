<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

The oscillator operators satisfy $[a,a^\dagger]=1$ and $[a,a]=[a^\dagger,a^\dagger]=0$. Substitution into the kinetic and potential energies gives

$$
\boxed{H=\hbar\omega(a^\dagger a+\tfrac12).}
$$

The [number operator](../../../../../number-operator.md) $N=a^\dagger a$ is nonnegative because $\langle\psi,N\psi\rangle=\|a\psi\|^2$. The commutators $[N,a]=-a$ and $[N,a^\dagger]=a^\dagger$ lower and raise an [eigenvalue](../../../../../eigenvalue.md) by one. If an [eigenvalue](../../../../../eigenvalue.md) were a noninteger $\nu\geq0$, repeated lowering would produce a nonzero [eigenvector](../../../../../eigenvector.md) with [eigenvalue](../../../../../eigenvalue.md) between zero and one, and one further lowering would have negative [eigenvalue](../../../../../eigenvalue.md); its [norm](../../../../../norm.md) is nonzero because $\|a\psi\|^2=\nu\|\psi\|^2$. This contradicts nonnegativity. Thus only nonnegative integers are allowed. The normalized Gaussian solves $a|0\rangle=0$, and raising it supplies every level, with

$$
\boxed{E_n=\hbar\omega(n+\tfrac12),\qquad
|n\rangle=(a^\dagger)^n|0\rangle/\sqrt{n!}.}
$$

For the three-dimensional unperturbed oscillator the product states are $|n_1,n_2,n_3\rangle=|n_1\rangle\otimes|n_2\rangle\otimes|n_3\rangle$, with energy $\hbar\omega(n_1+n_2+n_3+3/2)$.

Write the perturbation as $\lambda W$, where $W=(\hbar\omega/2)\sum_{i<j}(a_i+a_i^\dagger)(a_j+a_j^\dagger)$. Its ground-state expectation is zero. Acting on the [ground state](../../../../../ground-state.md), it produces $|110\rangle,|101\rangle,|011\rangle$, each with coefficient $\hbar\omega/2$. They lie $2\hbar\omega$ above the [ground state](../../../../../ground-state.md), so second-order [perturbation theory](../../../../../perturbation-theory.md) gives

$$
\boxed{E_{\rm ground}=\tfrac32\hbar\omega-\tfrac38\lambda^2\hbar\omega+O(\lambda^3).}
$$

In the first excited subspace with basis $|100\rangle,|010\rangle,|001\rangle$, the first-order perturbation [matrix](../../../../../matrix.md) is $(\lambda\hbar\omega/2)\begin{pmatrix}0&1&1\\1&0&1\\1&1&0\end{pmatrix}$. Its symmetric [eigenvector](../../../../../eigenvector.md) has [eigenvalue](../../../../../eigenvalue.md) $\lambda\hbar\omega$, while the perpendicular two-dimensional space has [eigenvalue](../../../../../eigenvalue.md) $-\lambda\hbar\omega/2$. Thus the lowest excited triplet splits into

$$
\boxed{\tfrac52\hbar\omega+\lambda\hbar\omega+O(\lambda^2)\quad\text{once},\qquad
\tfrac52\hbar\omega-\tfrac12\lambda\hbar\omega+O(\lambda^2)\quad\text{twice}.}
$$

As an independent check, diagonalizing the quadratic potential gives normal frequencies $\omega\sqrt{1+2\lambda}$ and $\omega\sqrt{1-\lambda}$ twice; their small-$\lambda$ expansions reproduce both results.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
