<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A dispatch cycle contains $N$ interarrival times and has mean length $N/\mu$. The expected total passenger waiting time in one cycle is

$$
\frac1\mu(1+2+\cdots+(N-1))=\frac{N(N-1)}{2\mu}.
$$

The renewal-reward average cost rate is therefore

$$
C(N)=\frac{K+cN(N-1)/(2\mu)}{N/\mu}
=\frac{\mu K}{N}+\frac c2(N-1).
$$

Thus the continuous optimum is $\sqrt{2\mu K/c}$, and the integer optimum is the positive integer minimizing $C(N)$; equivalently it is the smallest $N$ with

$$
N(N+1)\geq\frac{2\mu K}{c},
$$

with both adjacent values optimal in the equality case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
