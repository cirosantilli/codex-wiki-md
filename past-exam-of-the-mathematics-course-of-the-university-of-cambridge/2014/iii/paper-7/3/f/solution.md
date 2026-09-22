<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

If $f$ and $\widetilde f$ are two weak solutions with the same initial value and the required local time bound, their difference $w$ satisfies $w=\tau w$. By [linearity](../../../../../../linearity.md) this implies $w=\tau^nw$ for every $n$. On $[0,T]$ put $A_T=\sup_{s\leq T}\|w(s)\|_1<\infty$. The [factorial bound for a Volterra iterate](../../../../../../factorial-bound-for-a-volterra-iterate.md) now gives

$$
 \|w(t)\|_1\leq A_T\frac{(2T)^n}{n!},\qquad0\leq t\leq T.
$$

For fixed $T$, the factor tends to zero; its successive-term ratio is $2T/(n+1)$. Therefore $w(t)=0$ as an $L^1$ element at every time on this interval. Since $T$ is arbitrary, **the locally time-bounded $L^1$ weak solution is unique globally**. This proof uses precisely the additional condition requested, rather than assuming arbitrary pointwise-in-time integrability alone supplies a finite uniform bound.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
