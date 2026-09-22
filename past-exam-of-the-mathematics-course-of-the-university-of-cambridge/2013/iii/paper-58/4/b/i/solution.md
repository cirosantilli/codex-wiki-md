<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [unitary operator](../../../../../../../unitary-operator.md) $W$, $WW^\dagger=I$. Thus for every nonnegative integer $j$,

$$
(W^\dagger H W)^j=W^\dagger H^jW.
$$

Insert this into the convergent [matrix exponential](../../../../../../../matrix-exponential.md) series in the finite-dimensional qubit setting:

$$
W^\dagger e^{iH}W=\sum_{j=0}^\infty\frac{i^j}{j!}W^\dagger H^jW=\sum_{j=0}^\infty\frac{i^j}{j!}(W^\dagger HW)^j.
$$

**Consequently unitary conjugation commutes with the exponential:**

$$
\boxed{W^\dagger e^{iH}W=e^{iW^\dagger HW}.}
$$

For an unbounded self-adjoint [Hamiltonian](../../../../../../../hamiltonian.md), the same identity follows from the [spectral theorem for normal operators](../../../../../../../spectral-theorem-for-normal-operators.md), with the domain transported by $W$; no unbounded power-series manipulation is needed.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 58](../../../../paper-58-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
