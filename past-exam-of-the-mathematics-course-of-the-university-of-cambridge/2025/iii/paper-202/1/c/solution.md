<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply part (a)'s square formula, extended by the [Jordan decomposition of a function of bounded variation](../../../../../../jordan-decomposition-of-a-function-of-bounded-variation.md) from nondecreasing functions to arbitrary càdlàg functions of [bounded variation](../../../../../../total-variation-of-a-function.md), to $f+g$, $f$, and $g$. Since

$$
fg=\frac12\bigl((f+g)^2-f^2-g^2\bigr),
$$

linearity of the [Lebesgue-Stieltjes integral](../../../../../../lebesgue-stieltjes-integration.md) leaves $\int_0^tf\,dg+\int_0^tg\,df$. At each time $s$, polarization of the jump correction gives

$$
\frac12\left((\Delta f(s)+\Delta g(s))^2-\Delta f(s)^2-\Delta g(s)^2\right)
=\Delta f(s)\Delta g(s).
$$

Only common jump times contribute, and hence

$$
\boxed{f(t)g(t)=f(0)g(0)+\int_0^tf\,dg+\int_0^tg\,df
-\sum_{s\in A_f\cap A_g\cap(0,t]}\Delta f(s)\Delta g(s).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
