<h1 id="9f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

This is the unit-rate [Erlang distribution](../../../../../../erlang-distribution.md). For completeness, use convolution. The result is clear for $n=1$. If

$$
f_n(x)=\frac{x^{n-1}}{(n-1)!}e^{-x}\mathbf1_{\{x>0\}},
$$

then independence and the unit exponential density give, for $x>0$,

$$
\begin{aligned}
f_{n+1}(x)
&=\int_0^xf_n(y)e^{-(x-y)}\,dy\\
&=\frac{e^{-x}}{(n-1)!}\int_0^xy^{n-1}\,dy
=\frac{x^n}{n!}e^{-x}.
\end{aligned}
$$

Induction therefore proves

$$
\boxed{f_{X_n}(x)=\frac{x^{n-1}}{(n-1)!}e^{-x}},
\qquad x>0.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
