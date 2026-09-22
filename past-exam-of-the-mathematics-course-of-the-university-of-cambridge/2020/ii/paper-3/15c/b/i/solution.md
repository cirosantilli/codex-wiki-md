<h1 id="15c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Starting from $|0^n\rangle|0^n\rangle$, the first layer of [Hadamard gates](../../../../../../../hadamard-gate.md) gives

$$
2^{-n/2}\sum_{x\in B_n}|x\rangle|0^n\rangle.
$$

The [Boolean quantum oracle](../../../../../../../boolean-quantum-oracle.md) then gives

$$
2^{-n/2}\sum_{x\in B_n}|x\rangle|f(x)\rangle.
$$

Using the [Walsh-Hadamard transform](../../../../../../../walsh-hadamard-transform.md) identity

$$
H^{\otimes n}|x\rangle
=2^{-n/2}\sum_{y\in B_n}(-1)^{x\cdot y}|y\rangle,
$$

the final state is

$$
\boxed{2^{-n}\sum_{x,y\in B_n}(-1)^{x\cdot y}|y\rangle|f(x)\rangle.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [15C](../../../15c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
