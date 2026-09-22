<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Boltzmann factor](../../../../boltzmann-factor.md) factorizes over bonds. Define the [spin-chain transfer matrix](../../../../transfer-matrix-for-a-classical-spin-chain.md) by

$$
T_{ab}=e^{\beta J\delta_{ab}}
=1+(e^{\beta J}-1)\delta_{ab},\qquad a,b=1,\ldots,Q.
$$

Here $\delta_{ab}$ is the [Kronecker delta](../../../../kronecker-delta.md). Summing the product of these [matrix elements](../../../../matrix-element.md) over all configurations, and closing the final bond by [periodic boundary conditions](../../../../periodic-boundary-conditions.md), gives the [canonical partition function](../../../../canonical-partition-function.md)

$$
Z=\sum_{\sigma_1,\ldots,\sigma_L}
T_{\sigma_1\sigma_2}\cdots T_{\sigma_L\sigma_1}
=\operatorname{Tr}T^L.
$$

Hence, writing $I$ for the [identity matrix](../../../../identity-matrix.md) and $P$ for the [all-ones matrix](../../../../all-ones-matrix.md),

$$
\boxed{T=g(\beta J)I+P,\qquad g(\beta J)=e^{\beta J}-1.}
$$

Every element of $P^2$ is a sum of $Q$ ones, while every diagonal element of $P$ is one. Thus

$$
\boxed{P^2=QP,\qquad \operatorname{Tr}P=Q.}
$$

More explicitly, for $u=(1,\ldots,1)^T$, $Pu=Qu$. If $\sum_a v_a=0$, then $Pv=0$. These complementary [eigenspaces](../../../../eigenspace.md) have [dimensions](../../../../dimension-vector-space.md) $1$ and $Q-1$. Equivalently, $P/Q$ is the [orthogonal projector](../../../../orthogonal-projection.md) onto the [linear span](../../../../linear-span.md) of $u$. The [eigenvalues](../../../../eigenvalue.md) and their [eigenvalue multiplicities](../../../../eigenvalue-multiplicity.md) are therefore

$$
\boxed{\begin{aligned}
P:&\quad Q\ (1),\qquad 0\ (Q-1),\\
T:&\quad \lambda_+=e^{\beta J}+Q-1\ (1),\qquad
\lambda_-=e^{\beta J}-1\ (Q-1).
\end{aligned}}
$$

Since the two [matrices](../../../../matrix.md) share these [eigenvectors](../../../../eigenvector.md), the exact finite-ring [canonical partition function](../../../../canonical-partition-function.md) is

$$
\boxed{Z=(e^{\beta J}+Q-1)^L+(Q-1)(e^{\beta J}-1)^L.}
$$

Both terms matter in the finite-ring low-[temperature](../../../../temperature-split.md) limit: discarding the second would lose the correct [ground state](../../../../ground-state.md) [degeneracy factor](../../../../degeneracy-factor.md) and introduce a spurious single-wall contribution.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
