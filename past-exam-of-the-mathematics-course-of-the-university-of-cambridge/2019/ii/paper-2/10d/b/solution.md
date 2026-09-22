<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Alice sends the $m$ conjugate-coded [qubits](../../../../../../qubit.md) through the noiseless [quantum channel](../../../../../../quantum-channel.md). Bob independently chooses a uniformly random basis bit $y_i'$ for each qubit and performs a [projective measurement](../../../../../../projective-measurement.md) in the computational basis when $y_i'=0$ or the Hadamard basis when $y_i'=1$.

After all measurements, Alice and Bob publicly reveal $Y$ and $Y'$ but keep the data bits secret. They discard every position with $y_i\ne y_i'$ and retain the measured bits at positions where the bases agree. In the ideal channel those retained bits equal Alice's $x_i$ with certainty. Each pair of bases agrees with probability $1/2$, so the shared secret key has expected length $m/2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
