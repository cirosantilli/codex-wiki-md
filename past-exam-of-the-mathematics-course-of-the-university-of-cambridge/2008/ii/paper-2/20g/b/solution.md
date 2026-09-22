<h1 id="20g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Units have norm $\pm1$. Norm $-1$ is impossible modulo three. The least positive unit greater than one is

$$
\boxed{\varepsilon=11+2\sqrt{30}.}
$$

Indeed its norm is one. A smaller positive norm-one unit would have $0<y=(\varepsilon'-1/\varepsilon')/(2\sqrt{30})<2$, forcing $y=1$, but then $x^2=31$. Multiplying an arbitrary positive unit by powers of $\varepsilon$ reduces it to $[1,\varepsilon)$, so minimality proves that all units are $\pm\varepsilon^n$.

The equation with right side $+5$ is impossible modulo three, since it would require $x^2\equiv2\pmod3$. For norm $-5$, let $\beta=5+\sqrt{30}$, so $\beta^2=5\varepsilon$ and $\beta/\varepsilon=\sqrt{30}-5$. For [unit reduction for quadratic norm equations](../../../../../../unit-reduction-for-quadratic-norm-equations.md), change the sign of $x+y\sqrt{30}$ if necessary to make it positive, then multiply by a power of the [fundamental unit](../../../../../../fundamental-unit-number-theory.md) to place it in $[\beta/\varepsilon,\beta)$. Its conjugate is $-5$ divided by itself, so

$$
y=\frac{a+5/a}{2\sqrt{30}}\le1,\qquad y>0.
$$

The maximum on this interval occurs at its endpoints. Thus $y=1$, and $x^2=25$; only $x=-5$ lies in the half-open interval. Reversing the reduction gives all solutions:

$$
\boxed{x+y\sqrt{30}=\pm(5+\sqrt{30})(11+2\sqrt{30})^n,\qquad n\in\mathbb Z.}
$$

Every displayed element has norm $-5$, and the reduction proves completeness, including both signs of $x$ and $y$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20G](../../20g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
