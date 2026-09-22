<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The coefficient formula from part (b) and the [Leibniz rule](../../../../../leibniz-rule.md) yield [Rodrigues' formula](../../../../../rodrigues-formula.md) directly:

$$
p_n(x)=\sum_{j=0}^n\frac{(-1)^j}{j!}\binom njx^j
=\frac{e^x}{n!}\frac{d^n}{dx^n}(e^{-x}x^n).
$$

The leading coefficient is $(-1)^n/n!$, so $p_n^{(n)}=(-1)^n$. Substitute this differentiated expression into one factor in the squared [weighted norm](../../../../../weighted-norm.md) and apply [integration by parts](../../../../../integration-by-parts.md) $n$ times:

$$
\begin{aligned}
\|p_n\|_w^2
&=\frac1{n!}\int_0^\infty p_n(x)\frac{d^n}{dx^n}(e^{-x}x^n)\,dx\\
&=\frac{(-1)^n}{n!}\int_0^\infty e^{-x}x^n p_n^{(n)}(x)\,dx
=\frac1{n!}\int_0^\infty e^{-x}x^n\,dx
=\boxed{1}.
\end{aligned}
$$

Every endpoint term contains a derivative of $e^{-x}x^n$ of order less than $n$: it vanishes at zero, and its exponential decay beats every [polynomial](../../../../../polynomial-split.md) at infinity. This proves the [normalization of the ordinary Laguerre polynomials](../../../../../normalization-of-the-ordinary-laguerre-polynomials.md) for all $n$, including $n=0$ without any integrations by parts.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
