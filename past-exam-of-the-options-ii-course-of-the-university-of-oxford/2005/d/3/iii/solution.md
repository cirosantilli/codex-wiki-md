<h1 id="d/3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use $|\sin(\alpha x)|\le|\alpha|x$ for $x\ge0$. For the source's functions,

$$
\int_{\mathbb R}|f_n(x)|\,dx
\le|\alpha|\int_0^\infty xe^{-nx}\,dx=\frac{|\alpha|}{n^2}.
$$

The last [integral](../../../../../integral-split.md) follows by the substitution $u=nx$ and [integration by parts](../../../../../integration-by-parts.md). Since $\sum_n n^{-2}$ converges, (ii) permits summing the [integrals](../../../../../integral-split.md) and identifies an integrable almost-everywhere sum.

For every $x>0$, the [geometric series](../../../../../geometric-series.md) gives

$$
\sum_{n=1}^\infty e^{-nx}\sin(\alpha x)
=\frac{\sin(\alpha x)}{e^x-1}.
$$

The functions vanish on $x\le0$, and the single endpoint does not change the [integral](../../../../../integral-split.md). Use the supplied [integral](../../../../../integral-split.md) of $f_n$ to obtain

$$
\boxed{\int_0^\infty\frac{\sin(\alpha x)}{e^x-1}\,dx
=\sum_{n=1}^\infty\frac{\alpha}{\alpha^2+n^2}.}
$$

The estimates include negative $\alpha$ through its absolute value, and the case $\alpha=0$ gives zero on both sides.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [D](../../../d.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
