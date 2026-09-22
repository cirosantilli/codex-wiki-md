<h1 id="6/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Termwise differentiation of the absolutely convergent [matrix exponential](../../../../../../matrix-exponential.md) series gives

$$
\frac{d}{dt}e^{tP}=e^{tP}P=Pe^{tP}.
$$

Because $P$ and $Q$ [commute](../../../../../../commuting-elements.md), $P$ also [commutes](../../../../../../commuting-elements.md) with every power of $Q$ and hence with $e^{tQ}$. The [product rule](../../../../../../product-rule.md) therefore gives

$$
f_1'(t)=e^{tP}Pe^{tQ}+e^{tP}e^{tQ}Q=f_1(t)(P+Q).
$$

Direct differentiation gives $f_2'(t)=f_2(t)(P+Q)$, and both initial values are $I$. The [uniqueness theorem for ordinary differential equations](../../../../../../uniqueness-theorem-for-ordinary-differential-equations.md), applied to the finitely many [matrix](../../../../../../matrix.md) entries, implies $f_1=f_2$. One can see uniqueness directly: the difference $D=f_1-f_2$ obeys $D'=D(P+Q)$ and $D(0)=0$, so

$$
\frac{d}{dt}\left(De^{-t(P+Q)}\right)=0
$$

and the product is identically zero. At $t=1$ this yields

$$
\boxed{e^Pe^Q=e^{P+Q}\quad\text{when }PQ=QP.}
$$

## ↑ Ancestors (14)

1. [I](../i.md)
2. [D](../../d.md)
3. [6](../../../6.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
