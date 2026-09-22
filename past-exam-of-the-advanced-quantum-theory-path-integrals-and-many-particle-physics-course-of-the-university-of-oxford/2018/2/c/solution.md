<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $M=L/2$, so that the total number of [Ising spins](../../../../ising-spin-variable.md) is $3M$. Write $K=\beta J$ and group each triangle's two base spins and its apex into one cell. The [Ising chain with alternating triangular decorations](../../../../ising-chain-with-alternating-triangular-decorations.md) has a triangle bond followed by an undecorated connecting bond. Summing an apex [Ising spin](../../../../ising-spin-variable.md) first gives a decorated-bond [Boltzmann weight](../../../../boltzmann-factor.md)

$$
A_{st}=\sum_{\tau=\pm1}e^{-K[st+(s+t)\tau]}=2e^{-Kst}\cosh[K(s+t)].
$$

The undecorated bridge has [Boltzmann weight](../../../../boltzmann-factor.md) $B_{ts'}=e^{-Kts'}$. In the basis $+1,-1$,

$$
A=\begin{pmatrix}e^K+e^{-3K}&2e^K\\2e^K&e^K+e^{-3K}\end{pmatrix},\qquad
B=\begin{pmatrix}e^{-K}&e^K\\e^K&e^{-K}\end{pmatrix}.
$$

Each cell contributes $T=AB$, so [periodic boundary conditions](../../../../periodic-boundary-conditions.md) give

$$
\boxed{Z_L=\operatorname{Tr}(AB)^M.}
$$

The two [matrices](../../../../matrix.md) have common normalized [eigenvectors](../../../../eigenvector.md) $(1,1)^{\mathsf T}/\sqrt2$ and $(1,-1)^{\mathsf T}/\sqrt2$, expressing [spin inversion symmetry](../../../../spin-inversion-symmetry.md). Their respective [eigenvalues](../../../../eigenvalue.md) are

$$
a_+=3e^K+e^{-3K},\quad a_-=e^{-3K}-e^K,\qquad
b_+=e^{-K}+e^K,\quad b_-=e^{-K}-e^K.
$$

Consequently the cell [transfer matrix](../../../../transfer-matrix.md) has [eigenvalues](../../../../eigenvalue.md)

$$
\begin{aligned}
\lambda_+&=(3e^K+e^{-3K})(e^{-K}+e^K)=3+e^{-4K}+e^{-2K}+3e^{2K},\\
\lambda_-&=(e^{-3K}-e^K)(e^{-K}-e^K)=e^{-4K}-e^{-2K}-1+e^{2K},
\end{aligned}
$$

and the finite-size [partition function](../../../../canonical-partition-function.md) is

$$
\boxed{Z_L=\lambda_+^{L/2}+\lambda_-^{L/2}.}
$$

For $K>0$, $\lambda_-\geq0$ and $\lambda_+-\lambda_-=4+2e^{-2K}+2e^{2K}>0$, so only $\lambda_+$ survives in the [thermodynamic limit](../../../../thermodynamic-limit.md). Divide the [Helmholtz free energy](../../../../helmholtz-free-energy.md) by $3M$, the number of sites rather than the number of cells or base spins:

$$
\boxed{f(T)=-\frac{k_BT}{3}\ln\lambda_+
=-\frac{k_BT}{3}\ln\!\left(3+e^{-4\beta J}+e^{-2\beta J}+3e^{2\beta J}\right).}
$$

As a counting check, $K=0$ gives $\lambda_+=8$, $\lambda_-=0$, hence $Z_L=8^M=2^{3M}$, exactly the number of independent [Ising spin](../../../../ising-spin-variable.md) configurations. This model has separated decorated bonds and should not be confused with the corner-sharing [sawtooth Ising chain](../../../../sawtooth-ising-chain.md), which has a different site count.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
