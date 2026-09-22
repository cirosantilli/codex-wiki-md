<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [De Moivre's theorem](../../../../../de-moivre-s-theorem.md), $(e^{i\alpha})^j=e^{ij\alpha}$. The complex sum whose real part is wanted is therefore a [finite geometric series](../../../../../finite-geometric-series.md):

$$
Z=\sum_{j=0}^ne^{i(\theta+j\alpha)}
=e^{i\theta}\frac{1-e^{i(n+1)\alpha}}{1-e^{i\alpha}},
\qquad \alpha\notin2\pi\mathbb Z.
$$

Use $1-e^{i\beta}=-2ie^{i\beta/2}\sin(\beta/2)$ in the numerator and denominator. This yields

$$
Z=\frac{\sin((n+1)\alpha/2)}{\sin(\alpha/2)}
e^{i(\theta+n\alpha/2)}.
$$

Taking its real part proves the [finite trigonometric sum](../../../../../finite-trigonometric-sum.md)

$$
\boxed{\sum_{j=0}^n\cos(\theta+j\alpha)
=\frac{\sin((n+1)\alpha/2)}{\sin(\alpha/2)}
\cos\left(\theta+\frac{n\alpha}{2}\right).}
$$

When $\alpha\in2\pi\mathbb Z$, the printed quotient is undefined; the original sum is directly **$(n+1)\cos\theta$**, also the limiting value of the displayed identity. The denominator restriction cannot be omitted from a literal use of the quotient.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
