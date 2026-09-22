<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

The comparison test says that if $0\leq b_n\leq c_n$ eventually and $\sum c_n$ converges, then $\sum b_n$ converges. If $\sum a_nz_0^n$ converges, its terms are bounded: $|a_nz_0^n|\leq M$. For $|z_1|<|z_0|$,

$$
|a_nz_1^n|\leq M\left|\frac{z_1}{z_0}\right|^n,
$$

so comparison with a geometric [series](../../../../../series-mathematics.md) proves absolute convergence.

The radius $R$ is the number for which the power [series](../../../../../series-mathematics.md) converges absolutely for $|z|<R$ and diverges for $|z|>R$. Given $r_i<R_i$, both $\sum|a_n|r_1^n$ and $\sum|b_n|r_2^n$ converge, so their terms are bounded, say $|a_n|r_1^n\leq M$. Then

$$
\sum|a_nb_n|(r_1r_2)^n
\leq M\sum|b_n|r_2^n<\infty.
$$

**Thus $R\geq r_1r_2$; letting $r_i\uparrow R_i$ gives $R\geq R_1R_2$.**

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
