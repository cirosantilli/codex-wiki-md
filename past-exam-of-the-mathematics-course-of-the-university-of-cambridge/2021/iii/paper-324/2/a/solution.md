<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $m$ control qubits and [exact quantum phase estimation](../../../../../../exact-quantum-phase-estimation.md). A controlled $U^{2^j}$ on the unknown eigenstate can be synthesized from the available uncontrolled operation and the known eigenstate $|\xi_0\rangle$: conditionally swap $|\xi\rangle$ into an auxiliary register initialized to $|\xi_0\rangle$, apply $U^{2^j}$ to that register, and swap back. The auxiliary state is restored, while the control-one branch acquires $e^{2\pi i2^j\phi}$.

After Hadamard gates and these controlled powers, the control register is

$$
\frac1{2^{m/2}}\sum_{y=0}^{2^m-1}
e^{2\pi i cy/2^m}|y\rangle.
$$

The inverse [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) maps this state exactly to $|c\rangle$, so measurement determines $c$ with certainty. There are $m$ controlled swaps of $O(n)$ qubits, each promised power costs $\operatorname{poly}(n,j)$, and the inverse transform uses $O(m^2)$ elementary gates. The total cost is therefore $\operatorname{poly}(n,m)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
