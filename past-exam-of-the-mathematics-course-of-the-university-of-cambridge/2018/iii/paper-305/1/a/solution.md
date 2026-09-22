<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Minkowski metric](../../../../../../minkowski-metric.md) $g^{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ throughout. Taking the [Hermitian conjugation](../../../../../../hermitian-conjugation.md) of the massive [Dirac equation](../../../../../../dirac-equation.md) and using the [Dirac adjoint](../../../../../../dirac-adjoint.md) gives

$$
i(\partial_\mu\bar\psi)\gamma^\mu+m\bar\psi=0.
$$

Taking the [matrix transpose](../../../../../../transpose.md) and multiplying by the [charge conjugation](../../../../../../charge-conjugation.md) matrix $C$ yields

$$
iC\gamma^{\mu T}C^{-1}\partial_\mu(C\bar\psi^T)+mC\bar\psi^T=0,
\qquad
-i\gamma^\mu\partial_\mu\psi^c+m\psi^c=0.
$$

Thus the [charge conjugation of a Dirac field](../../../../../../charge-conjugation-of-a-dirac-field.md) preserves the free massive [Dirac equation](../../../../../../dirac-equation.md):

$$
\boxed{(i\gamma^\mu\partial_\mu-m)\psi^c=0.}
$$

The [unitarity](../../../../../../unitary-operator.md) of $C$ and $\gamma^0C^{-1}\gamma^0=-C^{-1}\gamma^{0T}$ also give

$$
\overline{\psi^c}=(C\bar\psi^T)^\dagger\gamma^0
=\psi^T\gamma^{0T}C^{-1}\gamma^0=-\psi^TC^{-1}.
$$

Consequently

$$
\boxed{\hat C\bar\psi(x)\hat C^{-1}=-\psi^T(x)C^{-1}.}
$$

Here $\hat C$ is the [unitary operator](../../../../../../unitary-operator.md) acting on the [relativistic quantum field](../../../../../../relativistic-quantum-field-split.md), whereas $C$ acts on [Dirac spinor](../../../../../../dirac-spinor.md) indices.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
