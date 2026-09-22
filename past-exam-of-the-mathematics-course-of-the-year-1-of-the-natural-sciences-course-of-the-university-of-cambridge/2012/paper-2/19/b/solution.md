<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<x<1$,

$$
\frac{x^b-1}{\ln x}=\int_0^b x^s\,ds.
$$

In particular its [absolute value](../../../../../absolute-value.md) is bounded by $|b|x^{\min(b,0)}$, proving convergence when $b>-1$; the apparent endpoint singularity at one is removable, with value $b$. On any compact parameter interval with lower bound $b_0>-1$, the differentiated integrand is $x^b$, dominated by $x^{b_0}$. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore justifies [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md):

$$
\boxed{J'(b)=\int_0^1x^b\,dx=\frac1{b+1}}.
$$

Hence $J(b)=\ln(b+1)+C$. Since the integrand is identically zero at $b=0$, $J(0)=0$ fixes $C=0$. Thus

$$
\boxed{J(b)=\ln(b+1),\qquad b>-1}.
$$

This proves the [logarithmic integral representation of the natural logarithm](../../../../../logarithmic-integral-representation-of-the-natural-logarithm.md), including its parameter range.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
