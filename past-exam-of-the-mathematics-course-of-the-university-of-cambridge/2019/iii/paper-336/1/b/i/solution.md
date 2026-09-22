<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $S(t)=a\sinh t-t$. For $a>1$, $S'(t)=a\cosh t-1>0$ on the integration interval, so its minimum is the endpoint $t=0$. The [Taylor series](../../../../../../../taylor-series.md) is

$$
S(t)=(a-1)t+\frac a6t^3+O(t^5).
$$

On the contributing scale $t=O(\nu^{-1})$, the higher terms are negligible. The endpoint form of [Laplace's method](../../../../../../../laplace-s-method.md), or the [Watson lemma](../../../../../../../watson-s-lemma.md), therefore gives

$$
\boxed{A_\nu(a\nu)\sim\int_0^\infty e^{-\nu(a-1)t}\,dt=\frac1{\nu(a-1)}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 336](../../../../paper-336-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
