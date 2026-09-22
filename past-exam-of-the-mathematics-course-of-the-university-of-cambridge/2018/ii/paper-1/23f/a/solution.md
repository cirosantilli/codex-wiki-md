<h1 id="23f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For every $t\geq0$, the fundamental theorem of calculus gives

$$
\varphi(t)=\int_0^t\varphi'(s)\,ds
=\int_0^\infty\varphi'(s)\mathbf1_{\{s<t\}}\,ds.
$$

Apply this with $t=|F(x)|$. Since the integrand is nonnegative, [Tonelli theorem](../../../../../../tonelli-theorem.md) permits exchanging the integrals:

$$
\begin{aligned}
\int_X\varphi(|F(x)|)\,d\mu(x)
&=\int_X\int_0^\infty
\varphi'(s)\mathbf1_{\{s<|F(x)|\}}\,ds\,d\mu(x)\\
&=\int_0^\infty\varphi'(s)
\mu(\{|F|>s\})\,ds.
\end{aligned}
$$

This is the generalized [layer cake representation](../../../../../../layer-cake-representation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [23F](../../23f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
