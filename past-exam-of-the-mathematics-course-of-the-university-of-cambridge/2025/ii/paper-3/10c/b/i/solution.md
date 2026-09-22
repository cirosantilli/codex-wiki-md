<h1 id="10c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $| -\rangle=(|0\rangle-|1\rangle)/\sqrt2$. Applying the oracle with this answer qubit produces phase kickback:

$$
U_f|x\rangle| -\rangle=(-1)^{f(x)}|x\rangle| -\rangle.
$$

Inside $A$, the $X$ gates on both search qubits conjugate the phase oracle for $11$. Hence

$$
A|x_1x_2\rangle| -\rangle
=(-1)^{[x_1x_2=00]}|x_1x_2\rangle| -\rangle
=I_0|x_1x_2\rangle| -\rangle,
$$

where $I_0=I-2|00\rangle\langle00|$.

The first oracle similarly acts on the search register as $I_{x_0}=I-2|x_0\rangle\langle x_0|$. Reading the remaining gates from right to left, the search-register operation after its initial Hadamards is therefore

$$
-Q=H^{\otimes2}I_0H^{\otimes2}I_{x_0},
$$

while the answer qubit remains in $| -\rangle$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [10C](../../../10c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
