<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the equation as $(L+\beta)y=-\cos x/x$ with the positive [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) from part (a). A [Sturm-Liouville eigenfunction expansion](../../../../../sturm-liouville-eigenfunction-expansion.md) therefore gives $a_n=-f_n/(4n^2+\beta)$, where weighted [orthogonal projection](../../../../../orthogonal-projection.md) gives

$$
f_n=\frac4\pi\int_0^{\pi/2}\sin(2nx)\cos x\,dx
=\frac{8n}{\pi(4n^2-1)}.
$$

Here the [product-to-sum formulas](../../../../../product-to-sum-formula.md) reduce the [integral](../../../../../integral-split.md) to half the sum of the integrals of $\sin((2n+1)x)$ and $\sin((2n-1)x)$. Consequently

$$
\boxed{y(x)=-\sum_{n=1}^\infty\frac{8n}{\pi(4n^2-1)(4n^2+\beta)}\frac{\sin(2nx)}x.}
$$

At $x=0$, use the continuous limits of the terms. The coefficients are $O(n^{-3})$, so the resulting endpoint series converges. Completeness is the ordinary [Fourier sine series](../../../../../fourier-sine-series.md) completeness after $v=xy$. For an independent check, solving $v''-\beta v=\cos x$ with zero endpoint values gives

$$
y(x)=\frac{\sinh(\sqrt\beta(\pi/2-x))/\sinh(\sqrt\beta\pi/2)-\cos x}{(1+\beta)x}.
$$

Its numerator vanishes at zero, and it has the same [orthogonal projection](../../../../../orthogonal-projection.md) coefficients. Positivity of $L+\beta$ proves [uniqueness](../../../../../uniqueness.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
