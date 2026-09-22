<h1 id="14a/solution">Solution</h1>

↑ **Parent:** [14A](../14a.md)

For a function holomorphic on and inside a positively oriented simple closed contour $C$, the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) gives

$$
f(z)=\frac1{2\pi i}\int_C\frac{f(\zeta)}{\zeta-z}\,d\zeta,\qquad f^{(m)}(z)=\frac{m!}{2\pi i}\int_C\frac{f(\zeta)}{(\zeta-z)^{m+1}}\,d\zeta.
$$

If an [entire function](../../../../../entire-function.md) is bounded by $M$, apply the derivative formula on a radius-$R$ circle about any $z$ to obtain $|f'(z)|\leq M/R$. Letting $R\to\infty$ makes every derivative $f'(z)$ zero, so $f$ is constant. This proves [Liouville theorem](../../../../../liouville-theorem.md) directly.

For the given [meromorphic function](../../../../../meromorphic-function.md), the growth bound excludes poles outside the bounding disc. Its poles inside are finite in number, since poles cannot accumulate at a finite point of a meromorphic function. Subtract all their finite [principal parts](../../../../../principal-part-of-a-meromorphic-function.md):

$$
g(z)=f(z)-\sum_p\sum_{j=1}^{m_p}\frac{a_{p,-j}}{(z-p)^j}.
$$

The remainder is entire. The rational sum is $O(1/|z|)$ at infinity. If $n\geq0$, this makes $g(z)=O(|z|^n)$; the [Cauchy estimates](../../../../../cauchy-estimate.md) at zero give $|g^{(m)}(0)|\leq m!\,O(R^{n-m})$ for $m>n$, hence these derivatives vanish. Its Taylor series is a polynomial of degree at most $n$. If $n<0$, then $g\to0$ at infinity, so it is bounded and equals zero by Liouville. In both cases, adding back the principal parts proves

$$
\boxed{f\text{ is a rational function}.}
$$

This proof of [polynomial growth forces a meromorphic function to be rational](../../../../../polynomial-growth-forces-a-meromorphic-function-to-be-rational.md) includes negative integers $n$, not only the polynomial-growth case $n\geq0$.

## ↑ Ancestors (10)

1. [14A](../14a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
