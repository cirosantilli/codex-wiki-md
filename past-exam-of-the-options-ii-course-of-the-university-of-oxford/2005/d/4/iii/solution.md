<h1 id="d/4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For fixed real $t$, [multiplication](../../../../../multiplication.md) by $e^{itx}$ does not change the absolute value. The product integrability proved in (ii) therefore justifies [Fubini theorem](../../../../../fubini-s-theorem.md) in the following calculation. [Set](../../../../../set-split.md) $u=x-y$ in the inner [integral](../../../../../integral-split.md):

$$
\begin{aligned}
\widehat{g*h}(t)
&=\int_{\mathbb R}\int_{\mathbb R}g(x-y)h(y)e^{itx}\,dy\,dx\\
&=\int_{\mathbb R}h(y)\left[\int_{\mathbb R}g(x-y)e^{itx}\,dx\right]dy\\
&=\int_{\mathbb R}h(y)e^{ity}\left[\int_{\mathbb R}g(u)e^{itu}\,du\right]dy\\
&=\widehat g(t)\widehat h(t).
\end{aligned}
$$

Thus

$$
\boxed{\widehat{g*h}=\widehat g\,\widehat h.}
$$

The positive exponential convention in the source is used throughout; no normalization factor is introduced under that convention.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
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
