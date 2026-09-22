<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Factor the square root of the [stochastic exponential](../../../../../../../doleans-dade-exponential.md) as

$$
\sqrt{S_T}
=\sqrt{S_0}\,
\mathcal E\!\left(\frac12(M-M_0)\right)_T
\exp\!\left(-\frac18[M]_T\right).
$$

The stochastic exponential in this expression is a positive local martingale and hence a [supermartingale](../../../../../../../supermartingale.md), so its expectation is at most one. If $[M]_T\geq a$ almost surely, then

$$
\boxed{\mathbb E\sqrt{S_T}
\leq\sqrt{S_0}e^{-a/8}
\mathbb E\mathcal E\!\left(\frac12(M-M_0)\right)_T
\leq\sqrt{S_0}e^{-a/8}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
