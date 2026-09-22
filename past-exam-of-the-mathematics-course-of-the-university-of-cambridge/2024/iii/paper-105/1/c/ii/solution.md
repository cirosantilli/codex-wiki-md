<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $u\in W_0^{1,p}(U)$ and extend it by zero outside $U$. The [zero extension of W01](../../../../../../../zero-extension-of-w01.md) belongs to $W^{1,p}(\mathbb R^n)$ and the [Sobolev inequality](../../../../../../../sobolev-inequality.md) gives

$$
\|u\|_{L^{p^*}(U)}\leq C_S\|Du\|_{L^p(U)}.
$$

Because $U$ has finite measure, the [Holder inequality](../../../../../../../holder-inequality.md) gives

$$
\|u\|_{L^p(U)}
\leq |U|^{1/p-1/p^*}\|u\|_{L^{p^*}(U)}
\leq C\|Du\|_{L^p(U)}.
$$

Thus

$$
\|u\|_{W^{1,p}(U)}
\leq C'\|Du\|_{L^p(U)}.
$$

The reverse estimate follows directly from $\|Du\|_{L^p}\leq\|u\|_{W^{1,p}}$. After adjusting constants,

$$
\boxed{C\|Du\|_{L^p(U)}\leq\|u\|_{W^{1,p}(U)}\leq C'\|Du\|_{L^p(U)}}.
$$

This is the [Poincaré inequality](../../../../../../../poincare-inequality.md) on $W_0^{1,p}(U)$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
