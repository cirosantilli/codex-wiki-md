<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $K=\beta J$. The [transfer matrix for the one-dimensional Ising model](../../../../transfer-matrix-for-the-one-dimensional-ising-model.md) assigns a [Boltzmann factor](../../../../boltzmann-factor.md) to each bond. In the [Ising spin](../../../../ising-spin-variable.md) order $(+1,-1)$, it is

$$
T_{ss'}=e^{-Kss'},\qquad
T=\begin{pmatrix}e^{-K}&e^K\\e^K&e^{-K}\end{pmatrix}.
$$

Multiplying these bond factors and summing every [Ising spin](../../../../ising-spin-variable.md) implements the [canonical ensemble](../../../../canonical-ensemble-split.md). The [periodic boundary conditions](../../../../periodic-boundary-conditions.md) close the product into a [trace](../../../../matrix-trace.md):

$$
Z_N=\sum_{S_1,\ldots,S_N}\prod_{j=1}^NT_{S_jS_{j+1}}
=\operatorname{tr}T^N.
$$

The [eigenvectors](../../../../eigenvector.md) $|+\rangle=(1,1)^T/\sqrt2$ and $|-\rangle=(1,-1)^T/\sqrt2$ form an [orthonormal basis](../../../../orthonormal-basis.md), with [eigenvalues](../../../../eigenvalue.md)

$$
\lambda_+=e^{-K}+e^K=2\cosh K,
\qquad
\lambda_-=e^{-K}-e^K=-2\sinh K.
$$

The negative second [eigenvalue](../../../../eigenvalue.md) encodes alternating [correlations](../../../../pearson-correlation-coefficient.md). Defining $q=\lambda_-/\lambda_+=-\tanh K$, the exact [partition function](../../../../canonical-partition-function.md) and total [Helmholtz free energy](../../../../helmholtz-free-energy.md) are

$$
\boxed{Z_N=(2\cosh K)^N+(-2\sinh K)^N
=(2\cosh K)^N(1+q^N),}
$$



$$
\boxed{F_N=-\frac1\beta\ln Z_N
=-\frac N\beta\ln(2\cosh K)-\frac1\beta\ln(1+q^N).}
$$

The parity-dependent term must be retained for finite $N$; in particular it nearly cancels the leading term of $Z_N$ at low [temperature](../../../../temperature-split.md) when $N$ is odd.

Represent insertion of one [Ising spin](../../../../ising-spin-variable.md) by $\Sigma=\operatorname{diag}(1,-1)$. In the [eigenbasis](../../../../eigenbasis.md) of $T$, this [matrix](../../../../matrix.md) swaps $|+\rangle$ and $|-\rangle$. Its diagonal entries in that [eigenbasis](../../../../eigenbasis.md) vanish, giving the exact [one-point correlation function](../../../../one-point-correlation-function.md)

$$
\boxed{\langle S_1\rangle=\frac{\operatorname{tr}(\Sigma T^N)}{Z_N}=0.}
$$

Equivalently, configurations pair with their opposites under [spin inversion symmetry](../../../../spin-inversion-symmetry.md), with the same [Boltzmann factor](../../../../boltzmann-factor.md) and opposite $S_1$.

Two insertions separated by $n$ bonds give the [two-point correlation function](../../../../two-point-correlation-function.md)

$$
\begin{aligned}
\langle S_1S_{n+1}\rangle
&=\frac{\operatorname{tr}(\Sigma T^n\Sigma T^{N-n})}{Z_N}\\
&=\frac{\lambda_-^n\lambda_+^{N-n}+\lambda_+^n\lambda_-^{N-n}}
{\lambda_+^N+\lambda_-^N}.
\end{aligned}
$$

Thus the exact [finite antiferromagnetic Ising-ring correlation](../../../../finite-ring-antiferromagnetic-ising-correlation.md) is

$$
\boxed{C_N(n):=\langle S_1S_{n+1}\rangle
=\frac{q^n+q^{N-n}}{1+q^N},\quad q=-\tanh(\beta J),\quad0\leq n\leq N-1.}
$$

The two numerator terms represent the two arcs between the sites. The formula has $C_N(0)=1$ and $C_N(n)=C_N(N-n)$, as required by the [periodic boundary conditions](../../../../periodic-boundary-conditions.md). Since the [one-point correlation function](../../../../one-point-correlation-function.md) is zero, this is also the [connected correlation function](../../../../connected-correlation-function.md). At $K=0$, every [Ising spin](../../../../ising-spin-variable.md) is [independent](../../../../independent-random-variables.md), so $C_N(n)=0$ for distinct sites and $C_N(0)=1$; powers with exponent zero are understood as one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the field theories and collective phenomena in condensed matter course of the University of Oxford](../../../split.md)
5. [Field theories and collective phenomena in condensed matter course of the University of Oxford](../../../../field-theories-and-collective-phenomena-in-condensed-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
