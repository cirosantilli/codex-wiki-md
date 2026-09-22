<h1 id="22f/solution">Solution</h1>

↑ **Parent:** [22F](../22f.md)

For a nonconstant [holomorphic map](../../../../../holomorphic-map.md) between [compact Riemann surfaces](../../../../../compact-riemann-surface.md), choose local coordinates making the map $z\mapsto z^{e_p}$. Its local degree is $e_p$, and its ramification excess is $e_p-1$; branching order conventions use either of these quantities, so both are specified below. The degree $d$ is the number of inverse images of any regular value, or the sum of local degrees in any fiber. The [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) is $2g_X-2=d(2g_Y-2)+\sum_p(e_p-1)$.

The projective closure is $S^m-T^m-Z^m=0$. Its three partial derivatives cannot vanish simultaneously at any projective point, so it is nonsingular and inherits the complex structure of a smooth projective curve. The affine polynomial is irreducible by Eisenstein applied to $t^m-(s^m-1)$ at the prime $s-1$ in $\mathbb C[s]$, so the smooth projective curve is connected. At $Z=0$ its points are $[\zeta:1:0]$, where $\zeta^m=1$; these are exactly the $m$ points added at infinity.

The extension of the coordinate projection is $F=[S:Z]$. There is no point on the curve with $S=Z=0$, so this gives a [holomorphic map](../../../../../holomorphic-map.md) everywhere. More explicitly, in the chart $T=1$ put $\sigma=S/T$, $\tau=Z/T$. Near an infinity point, $\sigma^m=1+\tau^m$ and $\sigma(0)=\zeta\ne0$. Thus $\tau$ is a local coordinate and $1/F=\tau/\sigma$ has nonzero derivative $1/\zeta$ at zero. Each infinity point is unramified, with local degree one.

For a generic finite $s$, there are $m$ distinct solutions of $t^m=s^m-1$, so $\deg F=m$. Ramification occurs exactly at $t=0$, $s^m=1$. At each such point, $t$ is a local coordinate and $s-s_0=t^m/(m s_0^{m-1})+O(t^{2m})$, giving local degree $m$ and ramification excess $m-1$. There are no other critical points, since away from $t=0$ the projection $s$ is a local coordinate. Therefore

$$
2g-2=-2m+m(m-1),\qquad\boxed{g=\frac{(m-1)(m-2)}2.}
$$

## ↑ Ancestors (10)

1. [22F](../22f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
