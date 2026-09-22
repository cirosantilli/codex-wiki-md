<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $Y(\theta)=y(\cos\theta)$, with $0<\theta<\pi$. The [chain rule](../../../../../chain-rule.md) gives

$$
y'=-\frac{Y'}{\sin\theta},\qquad
y''=\frac{Y''}{\sin^2\theta}-\frac{\cos\theta}{\sin^3\theta}Y'.
$$

Consequently the original differential expression becomes $-Y''-2\cot\theta\,Y'$. If $Y=F/\sin\theta$, direct differentiation gives

$$
Y''+2\cot\theta\,Y'=\frac{F''+F}{\sin\theta}.
$$

Taking $F=\sin n\theta$ therefore yields

$$
-Y''-2\cot\theta\,Y'=(n^2-1)Y,
\qquad
\boxed{y_n(x)=\frac{\sin(n\arccos x)}{\sqrt{1-x^2}}.}
$$

The apparent endpoint singularities are removable. Expansion at $\theta=0,\pi$ gives

$$
\begin{aligned}
y_n(1)&=n,&y_n(-1)&=(-1)^{n-1}n,\\
y_n'(1)&=\frac{n(n^2-1)}3,&y_n'(-1)&=(-1)^n\frac{n(n^2-1)}3.
\end{aligned}
$$

Thus both endpoint regularity conditions hold. This is the [Chebyshev polynomial of the second kind](../../../../../chebyshev-polynomial-of-the-second-kind.md) $U_{n-1}(x)$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
