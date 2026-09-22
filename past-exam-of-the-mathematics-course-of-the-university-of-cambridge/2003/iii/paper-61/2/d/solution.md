<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the spectral measure to have $n$ point masses at $k_j=i\kappa_j$, with distinct $\kappa_j>0$ and positive weights $c_j$. Set

$$
E_j=e^{-\kappa_jx+\kappa_j^3t},\qquad \Phi_j=\varphi(i\kappa_j,x,t).
$$

Evaluating the [linear integral equation](../../../../../../linear-integral-equation.md) at these points gives the explicit algebraic system and reconstruction

$$
\boxed{\Phi_i+\sum_{j=1}^n\frac{c_jE_i}{\kappa_i+\kappa_j}\Phi_j=E_i,\qquad
q=-\partial_x\sum_{j=1}^nc_j\Phi_j.}
$$

The sign is fixed by $i/(i\kappa_i+i\kappa_j)=1/(\kappa_i+\kappa_j)$. No continuum integration remains.

There is also a useful determinant form. Define $A_{ij}=c_jE_i/(\kappa_i+\kappa_j)$, $B=I+A$, $\tau=\det B$ and $\Lambda=\operatorname{diag}(\kappa_1,\ldots,\kappa_n)$. Then $A_x=-\Lambda A$ and $\Lambda A+A\Lambda=Ec^T$. Using the derivative of a [determinant](../../../../../../determinant.md) and cyclicity of the [trace](../../../../../../matrix-trace.md),

$$
\partial_x\log\tau=-\operatorname{tr}(B^{-1}\Lambda A)
=-\tfrac12\operatorname{tr}[B^{-1}(\Lambda A+A\Lambda)]
=-\tfrac12c^TB^{-1}E.
$$

Hence the [finite-rank KdV dressing determinant](../../../../../../finite-rank-kdv-dressing-determinant.md) gives

$$
\boxed{q=2\partial_x^2\log\tau.}
$$

Positivity ensures a regular real solution: the [Cauchy matrix](../../../../../../cauchy-matrix.md) $C_{ij}=1/(\kappa_i+\kappa_j)$ is the Gram matrix of the independent functions $e^{-\kappa_i s}$ on $s>0$, so it is positive definite. The matrix $A=\operatorname{diag}(E)C\operatorname{diag}(c)$ is diagonally similar to $\operatorname{diag}(\sqrt{cE})C\operatorname{diag}(\sqrt{cE})$. Its eigenvalues are positive, and $\tau>0$. The resulting reflectionless [multisoliton solution](../../../../../../multisoliton-solution.md) has $n$ distinct scales and velocities; the weights fix their positions. Arbitrary signed or complex weights need not give a nonsingular real solution.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
