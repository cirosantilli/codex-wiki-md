<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $D_\theta=\operatorname{diag}(1,e^{i\theta})$. Factoring the target operator gives

$$
U=D_\theta\otimes V,
$$

whereas $U'=I\otimes V$. Their difference is a [relative phase](../../../../../../relative-quantum-phase.md) on the first [qubit](../../../../../../qubit.md), not one overall [global phase](../../../../../../global-phase.md).

For an explicit witness, choose the product input $|+\rangle\otimes|\chi\rangle$, with any normalized $|\chi\rangle$. The first-[qubit](../../../../../../qubit.md) outputs are respectively $(|0\rangle+e^{i\theta}|1\rangle)/\sqrt2$ and $|+\rangle$. A [Hadamard basis](../../../../../../hadamard-basis.md) measurement returns $+$ with [probabilities](../../../../../../probability.md)

$$
\cos^2(\theta/2)\quad\text{and}\quad1.
$$

These differ because $\theta$ is not a multiple of $2\pi$. **The two [unitary operators](../../../../../../unitary-operator.md) implement different [quantum channels](../../../../../../quantum-channel.md).** The [global phase](../../../../../../global-phase.md) of the conditional target operation has become a physically observable phase on its control.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
