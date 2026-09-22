<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $K=\beta J$, where $\beta=1/(k_BT)$ is the [inverse temperature](../../../../inverse-temperature.md), $T$ is [temperature](../../../../temperature-split.md) and $k_B$ is the [Boltzmann constant](../../../../boltzmann-constant.md). In the [canonical ensemble](../../../../canonical-ensemble-split.md), each [spin configuration](../../../../spin-configuration.md) has [probability](../../../../probability.md) $e^{-\beta H}/Z_N$. The nearest-neighbor [Boltzmann factors](../../../../boltzmann-factor.md) multiply, so the [spin-chain transfer matrix](../../../../transfer-matrix-for-a-classical-spin-chain.md), in the order $+1,-1$, is

$$
\mathsf T_{ss'}=e^{-Kss'},\qquad
\mathsf T=\begin{pmatrix}e^{-K}&e^K\\e^K&e^{-K}\end{pmatrix}.
$$

Multiplying its entries around the ring and summing over every [Ising spin](../../../../ising-spin-variable.md) yields the [partition function](../../../../canonical-partition-function.md):

$$
Z_N=\sum_{S_1,\ldots,S_N}\mathsf T_{S_1S_2}\cdots\mathsf T_{S_NS_1}
=\operatorname{tr}\mathsf T^N.
$$

The [trace](../../../../matrix-trace.md) implements the [periodic boundary conditions](../../../../periodic-boundary-conditions.md); replacing it by an endpoint sum would describe a different [partition function](../../../../canonical-partition-function.md). The normalized [eigenvectors](../../../../eigenvector.md) and corresponding [eigenvalues](../../../../eigenvalue.md) are

$$
|+\rangle=\frac1{\sqrt2}\binom11,\quad
|-\rangle=\frac1{\sqrt2}\binom1{-1},\qquad
\lambda_+=2\cosh K,\quad \lambda_-=-2\sinh K.
$$

The negative [eigenvalue](../../../../eigenvalue.md) is essential for the [antiferromagnetic Ising model](../../../../antiferromagnetic-ising-model.md). Introduce their ratio

$$
t=\frac{\lambda_-}{\lambda_+}=-\tanh K.
$$

The exact finite-$N$ [partition function](../../../../canonical-partition-function.md) and [Helmholtz free energy](../../../../helmholtz-free-energy.md) are

$$
\boxed{Z_N=(2\cosh K)^N+( -2\sinh K)^N
=(2\cosh K)^N(1+t^N),}
$$



$$
\boxed{F_N=-\frac1\beta\log Z_N
=-\frac N\beta\log(2\cosh K)-\frac1\beta\log(1+t^N).}
$$

For finite $K>0$, $|t|<1$, so $Z_N>0$ for both even and odd $N$. The last term retains the finite-ring effect of [geometric frustration](../../../../geometrical-frustration.md).

To insert an [Ising spin](../../../../ising-spin-variable.md) into this [trace](../../../../matrix-trace.md), use the [diagonal matrix](../../../../diagonal-matrix.md) $\mathsf S=\operatorname{diag}(1,-1)$. In the [eigenbasis](../../../../eigenbasis.md) of $\mathsf T$, it exchanges $|+\rangle$ and $|-\rangle$, and hence has vanishing diagonal entries. The [one-point correlation function](../../../../one-point-correlation-function.md) is therefore

$$
\boxed{\langle S_1\rangle=
\frac{\operatorname{tr}(\mathsf S\mathsf T^N)}{Z_N}=0.}
$$

The same conclusion follows directly from [spin inversion symmetry](../../../../spin-inversion-symmetry.md): reversing every [Ising spin](../../../../ising-spin-variable.md) preserves the [energy](../../../../energy-split.md) and the [Boltzmann factor](../../../../boltzmann-factor.md) while reversing $S_1$.

For the [two-point correlation function](../../../../two-point-correlation-function.md), the two insertions divide the ring into paths of $n$ and $N-n$ bonds. Thus

$$
C_n\equiv\langle S_1S_{n+1}\rangle
=\frac{\operatorname{tr}(\mathsf S\mathsf T^n\mathsf S\mathsf T^{N-n})}{Z_N}
=\frac{\lambda_-^n\lambda_+^{N-n}+\lambda_+^n\lambda_-^{N-n}}
{\lambda_+^N+\lambda_-^N}.
$$

In particular, the exact [finite-ring antiferromagnetic Ising correlation](../../../../finite-ring-antiferromagnetic-ising-correlation.md) is

$$
\boxed{C_n=\frac{t^n+t^{N-n}}{1+t^N},\qquad t=-\tanh(\beta J),\quad0\le n\le N-1.}
$$

Because the [one-point correlation functions](../../../../one-point-correlation-function.md) vanish, this is also the [connected correlation function](../../../../connected-correlation-function.md). It gives $C_0=1$ and $C_n=C_{N-n}$, as required by $S_1^2=1$ and exchanging the two paths around the ring. At $K=0$, distinct [Ising spins](../../../../ising-spin-variable.md) are independent and $C_n=0$ for $1\le n\le N-1$; $C_0=1$ is understood separately if a power $0^0$ occurs in the displayed expression.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
