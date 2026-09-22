<h1 id="2/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

As Boolean functions on edge indicators,

$$
g_m(x)=\neg\operatorname{CLIQUE}_{n,m}(\neg x).
$$

Thus $g_m$ is the [dual Boolean function](../../../../../../dual-boolean-function.md) of the clique function. Given a monotone circuit for $g_m$, swap every AND gate with an OR gate and swap the constants zero and one. [De Morgan's laws](../../../../../../de-morgan-s-laws.md) show that the resulting circuit has the same size and computes $\operatorname{CLIQUE}_{n,m}$. The lower bound from part (v), with the same choice of $m$, therefore applies to $g_m$.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
