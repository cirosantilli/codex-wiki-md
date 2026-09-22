<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [layer cake representation](../../../../../../layer-cake-representation.md), followed by the assumed tail bound and [Tonelli theorem](../../../../../../tonelli-theorem.md), gives

$$
\begin{aligned}
\int_X f_1^p\,d\mu&=p\int_0^\infty a^{p-1}\mu\{f_1>a\}\,da\\
&\leq p\int_0^\infty a^{p-2}\int_{\{g>a\}}g\,d\mu\,da\\
&=p\int_Xg(x)\int_0^{g(x)}a^{p-2}\,da\,d\mu(x)\\
&=\frac p{p-1}\int_Xg^p\,d\mu.
\end{aligned}
$$

All integrands are nonnegative, so this use of [Tonelli theorem](../../../../../../tonelli-theorem.md) is valid before finiteness of the left-hand side is known. Since $q=p/(p-1)$, the result is

$$
\boxed{\|f_1\|_p^p\leq q\|g\|_p^p}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
