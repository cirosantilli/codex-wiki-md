<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The essential requirement is an efficient [quantum state preparation](../../../../../../quantum-state-preparation.md) circuit $B$ satisfying

$$
B|0^n\rangle=|b\rangle
=\frac1{\|b\|}\sum_{j=0}^{N-1}b_j|j\rangle.
$$

A standard sufficient promise is that $b$ has only $\operatorname{poly}(\log N)$ nonzero components, with their positions and values classically computable to the required precision in $\operatorname{poly}(\log N)$ time, and with efficiently computable normalization. More structured dense vectors are also allowed whenever cumulative weights or an equivalent data-access oracle permit amplitude encoding in polylogarithmic time. Without such a promise, merely loading $N$ arbitrary classical entries already costs $\Omega(N)$ and removes the claimed exponential dependence on dimension.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
