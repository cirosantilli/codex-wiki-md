<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $T$ is future time to dementia from age 50, its survival function is

$$
\mathbb P(T>t)=
\begin{cases}
e^{-t/10},&0\leq t\leq10,\\
e^{-1}e^{-(t-10)/5},&t>10.
\end{cases}
$$

The [tail-sum formula for expectation](../../../../../../../tail-sum-formula-for-expectation.md) gives the expected future time alive without dementia:

$$
\mathbb ET
=\int_0^{10}e^{-t/10}\,dt
+\int_{10}^{\infty}e^{-1}e^{-(t-10)/5}\,dt
=10(1-e^{-1})+5e^{-1}
=\boxed{10-5e^{-1}}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
