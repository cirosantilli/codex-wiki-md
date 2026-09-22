<h1 id="30a/solution">Solution</h1>

↑ **Parent:** [30A](../30a.md)

In $I(\lambda)$ put $t=u/\sqrt\lambda$. Expanding the cubic exponential near the endpoint $t=0$ gives

$$
I(\lambda)\sim\lambda^{-\alpha-1/2}\sum_{n=0}^\infty\frac{(-1)^n}{n!\lambda^{n/2}}\int_0^\infty u^{2\alpha+3n}e^{-u^2}\,du.
$$

The substitution $v=u^2$ evaluates the coefficient using the [Gamma function](../../../../../gamma-function.md). Thus, numbering the first term by $n=0$,

$$
\boxed{I(\lambda)\sim\sum_{n=0}^\infty\frac{(-1)^n\Gamma(\alpha+(3n+1)/2)}{2n!\,\lambda^{\alpha+(n+1)/2}}.}
$$

For any fixed truncation the exponential's Taylor remainder is bounded by the next power times $e^{-u^2}$, and replacing the finite upper limit by infinity adds an exponentially small tail. This justifies the [asymptotic expansion](../../../../../asymptotic-expansion.md) for $\alpha>-1/2$.

For large $n$, the ratio of magnitudes of consecutive terms, by [Stirling's formula](../../../../../stirling-formula.md), is

$$
\frac{\Gamma(\alpha+(3n+4)/2)}{(n+1)\sqrt\lambda\,\Gamma(\alpha+(3n+1)/2)}
\sim\left(\frac32\right)^{3/2}\sqrt{\frac n\lambda}.
$$

The least term consequently has index $\boxed{n\sim8\lambda/27}$. An indexing convention starting at one changes this by one, without changing the estimate.

For the second integral, both endpoints minimize $t^2-t^3$. The endpoint $t=0$ gives the same expansion with positive coefficients. Its first two contributions are

$$
\boxed{J(\lambda)=\frac{\Gamma(\alpha+1/2)}{2\lambda^{\alpha+1/2}}+
\frac{\Gamma(\alpha+2)}{2\lambda^{\alpha+1}}+O(\lambda^{-1}),\quad-1/2<\alpha<0.}
$$

To check their ordering, near $t=1$ write $t=1-v/\lambda$. Then $\lambda(t^2-t^3)=v+O(v^2/\lambda)$ and $t^{2\alpha}=1+O(v/\lambda)$, producing a contribution $1/\lambda+O(\lambda^{-2})$. Because $\alpha+1<1$, this is smaller than the second displayed term. It is the third term, ahead of the next $t=0$ contribution of order $\lambda^{-\alpha-3/2}$. Splitting the integral into small endpoint neighborhoods and an interior interval, where the phase is strictly positive, makes the endpoint estimates rigorous.

## ↑ Ancestors (10)

1. [30A](../30a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
