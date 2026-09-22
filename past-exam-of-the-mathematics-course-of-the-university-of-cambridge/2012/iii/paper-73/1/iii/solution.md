<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use $A=S+\Omega$, where $S$ is the [rate-of-strain tensor](../../../../../../strain-rate-tensor.md) and $\Omega$ is antisymmetric. For [incompressible flow](../../../../../../incompressible-flow.md) $\operatorname{tr}S=0$. Since $\Omega^2=(\boldsymbol\omega\boldsymbol\omega^T-\omega^2I)/4$, taking a trace gives

$$
\operatorname{tr}A^3=\operatorname{tr}S^3+3\operatorname{tr}(S\Omega^2)
=\operatorname{tr}S^3+\frac34\omega_i\omega_jS_{ij}.
$$

This uses the positive convention $R=\operatorname{tr}A^3/3$ specified here; a convention with the opposite sign for $R$ must not be mixed into the calculation. For a compressible flow there is an additional term $-3\omega^2\operatorname{tr}S/4$, so the displayed incompressible formula is not literally valid for every flow.

One can exhibit the required divergence directly. Define

$$
F_i=u_j(\partial_j u_k)(\partial_k u_i)-\frac12u_i(\partial_j u_k)(\partial_k u_j).
$$

Differentiating, terms containing $\partial_i u_i$ vanish, and the two terms with a second derivative cancel after relabeling indices. Therefore

$$
\operatorname{tr}A^3=\partial_iF_i,\qquad \langle\operatorname{tr}A^3\rangle=0
$$

in [homogeneous turbulence](../../../../../../homogeneous-turbulence.md) with finite differentiable [moments](../../../../../../moment.md), or under periodic averaging. This is the [Betchov relation](../../../../../../betchov-relation.md). The preceding trace identity then implies

$$
\boxed{\langle\omega_i\omega_jS_{ij}\rangle=-\frac43\langle\operatorname{tr}S^3\rangle
=-\frac43\langle a^3+b^3+c^3\rangle}.
$$

The [principal strain rates](../../../../../../principal-strain-rates.md) are the real [eigenvalues](../../../../../../eigenvalue.md) of the [symmetric matrix](../../../../../../symmetric-matrix.md) $S$. Incompressibility gives $a+b+c=0$, and the identity $a^3+b^3+c^3-3abc=(a+b+c)(a^2+b^2+c^2-ab-bc-ca)$ gives

$$
\boxed{\langle\omega_i\omega_jS_{ij}\rangle=-4\langle abc\rangle}.
$$

No isotropy is required for this averaged tensor identity: [statistical homogeneity](../../../../../../statistical-homogeneity.md) and incompressibility are the key assumptions.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
