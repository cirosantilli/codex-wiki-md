<h1 id="22h/solution">Solution</h1>

↑ **Parent:** [22H](../22h.md)

A [meromorphic differential on a Riemann surface](../../../../../meromorphic-differential-on-a-riemann-surface.md) has local expression $\omega=a(z)dz$ with a meromorphic coefficient. On overlapping coordinates it transforms by $a(z)dz=\widetilde a(w)dw$. For a [meromorphic function](../../../../../meromorphic-function.md) $f$, the coefficients $f'(z)$ obey this transformation by the chain rule, so $df$ is such a differential. Two nonzero differentials have coefficient ratio $a/b$; the derivative factors cancel on overlaps, yielding a global [meromorphic function](../../../../../meromorphic-function.md) $h$ with $\eta=h\omega$.

An invertible holomorphic coordinate change has a nonzero holomorphic derivative, so multiplying by its derivative changes no local zero or [pole](../../../../../pole.md) order. Thus the differential's divisor is well defined. For a compact connected surface, the canonical-degree theorem states $\sum_P\operatorname{ord}_P\omega=2g-2$, including negative orders for [poles](../../../../../pole.md). Therefore $\boxed{g=1+\tfrac12\sum_P\operatorname{ord}_P\omega}$.

The projective closure has equation $U^2-V^2-W^2=0$. Its gradient $(2U,-2V,-2W)$ cannot vanish at a projective point, so it is nonsingular. At infinity $W=0$ gives the two points $[1:1:0]$ and $[1:-1:0]$. In the supplied sphere parameter,

$$
v(t)=\frac{2t}{t^2-1},\qquad dv=-\frac{2(t^2+1)}{(t^2-1)^2}\,dt.
$$

This has double [poles](../../../../../pole.md) at $t=\pm1$, the two infinity points, and simple zeros at $t=\pm i$. At the parameter infinity use $s=1/t$, giving $v=2s/(1-s^2)$ and $dv=2(1+s^2)(1-s^2)^{-2}ds$, which is regular and nonzero at $s=0$. Hence **$dv$ extends meromorphically over the whole projective curve**. Its order sum $2-4=-2$ gives genus zero, consistently with the stated biholomorphism from the sphere.

## ↑ Ancestors (10)

1. [22H](../22h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
