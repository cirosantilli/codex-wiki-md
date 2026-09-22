<h1 id="6b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a normalized [wavefunction](../../../../../../wave-function.md) in the required operator domains and a [self-adjoint operator](../../../../../../self-adjoint-operator.md) $A$, its [expectation value](../../../../../../expectation-value.md) and [standard deviation](../../../../../../standard-deviation.md) are

$$
\langle A\rangle_\psi=\int_{\mathbb R^3}\psi^*(\mathbf x)(A\psi)(\mathbf x)\,d^3x,
$$



$$
\Delta_\psi A=\left[\int_{\mathbb R^3}\psi^*(A-\langle A\rangle_\psi)^2\psi\,d^3x\right]^{1/2}.
$$

Equivalently the squared uncertainty is $\|(A-\langle A\rangle_\psi)\psi\|^2$, which is visibly nonnegative. Since the [expectation value](../../../../../../expectation-value.md) of a [self-adjoint operator](../../../../../../self-adjoint-operator.md) is real, expansion of the square and $\int|\psi|^2=1$ give

$$
\boxed{\Delta_\psi A=\sqrt{\langle A^2\rangle_\psi-\langle A\rangle_\psi^2}.}
$$

For a state not normalized to one, divide each defining expectation integral by $\int|\psi|^2$ before using this formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6B](../../6b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
