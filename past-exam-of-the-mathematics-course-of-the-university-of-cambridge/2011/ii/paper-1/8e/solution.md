<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

At $x=0$, both denominators are nonzero because $a\notin2\pi\mathbb Z$; they remain nonzero for every real $x\geq0$. The integrand is therefore bounded on each finite interval. At infinity its terms decay respectively as $O(e^{-(1+b)x})$ and $O(e^{-(1-b)x})$, so $0<b<1$ gives [absolute convergence](../../../../../absolute-convergence.md).

Set $t=e^{-x}$. The two integrals become

$$
I(a,b)=e^{-ia}\int_0^1\frac{t^b}{1-e^{-ia}t}\,dt
-e^{ia}\int_0^1\frac{t^{-b}}{1-e^{ia}t}\,dt.
$$

By the [Euler integral for the hypergeometric function](../../../../../euler-integral-for-the-hypergeometric-function.md) and the [Gamma function recurrence](../../../../../gamma-function-recurrence.md), $\int_0^1t^{s-1}/(1-zt)\,dt={}_2F_1(1,s;s+1;z)/s$ for $s>0$ and the indicated unit-circle values $z\ne1$. Hence

$$
\boxed{I(a,b)=\frac{e^{-ia}}{1+b}{}_2F_1(1,1+b;2+b;e^{-ia})
-\frac{e^{ia}}{1-b}{}_2F_1(1,1-b;2-b;e^{ia}).}
$$

The [Gauss hypergeometric functions](../../../../../hypergeometric-function.md) here use their continuation from the Euler integral, so no pole crosses the integration interval.

## ↑ Ancestors (11)

1. [8E](../8e.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
