<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [rejection sampling](../../../../../../rejection-sampling.md), independently generate a proposal $Y$ with density $g$ and a uniform $U$ on $(0,1)$. Accept $Y$ if $U\le f(Y)/(Mg(Y))$; otherwise generate a fresh independent pair and repeat. Set the ratio to zero on $g=0$ where necessarily $f=0$. The envelope condition makes the acceptance threshold at most one.

For any measurable set $A$, a single attempt satisfies

$$
\mathbb P(Y\in A,\text{ accepted})=\int_Ag(y)\frac{f(y)}{Mg(y)}dy
=\frac1M\int_Af(y)dy.
$$

Taking the whole space shows that acceptance has probability $1/M$. Conditioning on acceptance therefore gives density $f$. Repeating rejected independent attempts preserves that conditional law and terminates almost surely; the number of attempts is geometric with mean $M$.

For fixed proposal density, admissibility requires $M\ge\sup_{g(x)>0}f(x)/g(x)$ under the pointwise convention in the question. Since $1/M$ decreases with $M$, **the smallest valid envelope gives the greatest acceptance probability**:

$$
\boxed{M_* =\sup_{g(x)>0}\frac{f(x)}{g(x)},\qquad p_{\mathrm{acc}}=1/M_*.}
$$

For densities specified only almost everywhere, replace the supremum by the essential supremum. Integration of the envelope also gives $M\ge1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
