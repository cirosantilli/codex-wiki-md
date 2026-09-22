<h1 id="13/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [diagonalizable matrix](../../../../../diagonalizable-matrix.md), write $M=P\operatorname{diag}(\lambda_j)P^{-1}$. Relative to an existing [fixed point](../../../../../fixed-point.md),

$$
x_k-X=P\operatorname{diag}(\lambda_j^{k-1})P^{-1}(x_1-X).
$$

Convergence to the **same fixed point for every initial vector** therefore holds exactly when

$$
\boxed{|\lambda_j|<1\text{ for all }j,\quad\text{equivalently }\rho(M)<1.}
$$

Here $\rho(M)$ is the [spectral radius](../../../../../spectral-radius.md). Necessity follows by choosing an initial displacement in each [eigenspace](../../../../../eigenspace.md); sufficiency follows because every displayed scalar power tends to zero. The condition also makes $I-M$ an [invertible matrix](../../../../../invertible-matrix.md), so that [fixed point](../../../../../fixed-point.md) exists uniquely for every $c$.

If instead different initial vectors may converge to different constant solutions, an [eigenvalue](../../../../../eigenvalue.md) $1$ is allowed: all other [eigenvalues](../../../../../eigenvalue.md) must have [modulus](../../../../../modulus.md) less than one, and the component of $c$ in the [eigenspace](../../../../../eigenspace.md) for $1$ must vanish. That component of the initial vector then remains unchanged. No other unit-modulus [eigenvalue](../../../../../eigenvalue.md) is compatible with convergence for arbitrary initial vectors.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [13](../../../13.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
