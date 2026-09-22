<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Induct on $k$, using the recursive divided-difference formula. After substituting the two induction hypotheses, use

$$
f[t_1,\ldots,t_m]-f[t_0,\ldots,t_{m-1}]
=(t_m-t_0)f[t_0,\ldots,t_m]
$$

and the analogous identity for $g$; adjacent terms telescope. This proves

$$
\boxed{(fg)[t_0,\ldots,t_k]
=\sum_{m=0}^kf[t_0,\ldots,t_m]g[t_m,\ldots,t_k]}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
