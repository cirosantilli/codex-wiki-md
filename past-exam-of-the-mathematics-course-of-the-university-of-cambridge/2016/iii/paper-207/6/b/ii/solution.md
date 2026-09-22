<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An individual has neither died nor been censored by time $t$ exactly when $T>t$ and $C>t$. Under [independent censoring](../../../../../../../independent-censoring.md), this has probability $F_T(t)G(t)$. Thus **the probability of leaving observation by either route** is

$$
\boxed{\mathbb P(\min(T,C)\le t)=1-F_T(t)G(t)=\begin{cases}1-F_T(t),&0\le t<\tau_c-\tau_b,\\1-F_T(t)\dfrac{\tau_c-\tau_a-t}{\tau_b-\tau_a},&\tau_c-\tau_b\le t<\tau_c-\tau_a.\end{cases}}
$$

The two pieces agree at $t=\tau_c-\tau_b$. The expression counts the first of death and censoring, so it does not double-count individuals who would eventually experience both.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
