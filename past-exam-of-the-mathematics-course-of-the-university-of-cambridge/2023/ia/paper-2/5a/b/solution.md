<h1 id="5a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x>0$, division by $x$ gives

$$
y'-(2x+x^{-1})y=x.
$$

An integrating factor is $e^{-x^2}/x$, so

$$
y=xe^{x^2}\left(C+\int_0^xe^{-t^2}dt\right).
$$

Every choice except

$$
C=-\int_0^\infty e^{-t^2}dt=-\frac{\sqrt\pi}{2}
$$

grows like $xe^{x^2}$. The [bounded solution selected by a terminal condition](../../../../../../bounded-solution-selected-by-a-terminal-condition.md) is therefore

$$
y_b(x)=-xe^{x^2}\int_x^\infty e^{-t^2}dt.
$$

Integration by parts, or the Gaussian-tail asymptotic, gives

$$
\int_x^\infty e^{-t^2}dt\sim\frac{e^{-x^2}}{2x},
\qquad y_b(x)\to-\frac12.
$$

It starts from $0$ at $x=0$, remains negative, and decreases monotonically toward the horizontal asymptote $-1/2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5A](../../5a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
