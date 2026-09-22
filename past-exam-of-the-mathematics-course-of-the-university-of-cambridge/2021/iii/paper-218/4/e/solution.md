<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A dead ReLU unit has nonpositive preactivation for every training input, so its output and gradient are always zero. Replace $\max(0,z)$ by the leaky ReLU

$$
\phi_a(z)=\max(z,az),\qquad0<a<1.
$$

Its negative-side derivative $a$ permits recovery while it remains nonsaturating, preserving the gradient advantage over sigmoid activation.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
