<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

The planar [planar isoperimetric inequality](../../../../../planar-isoperimetric-inequality.md) is

$$
\boxed{4\pi A(\Omega)\leq l(\partial\Omega)^2},
$$

with equality precisely for a disc. Let the positively oriented boundary be parametrized by arclength as $r(s)=(x(s),y(s))$, $0\leq s\leq L$. Translate its mean to zero. Then $|r'|=1$, and [Green's theorem](../../../../../green-theorem.md) gives $2A=\int_0^L(xy'-yx')ds$.

The periodic [Wirtinger inequality](../../../../../wirtinger-inequality.md) says that for a real absolutely continuous $L$-periodic function $h$ of mean zero and square-integrable [derivative](../../../../../derivative.md),

$$
\int_0^Lh^2ds\leq\left(\frac L{2\pi}\right)^2\int_0^L(h')^2ds,
$$

with equality exactly for $h(s)=a\cos(2\pi s/L)+b\sin(2\pi s/L)$. Apply it to both coordinates and use [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md):

$$
2A\leq\left(\int|r|^2ds\right)^{1/2}\left(\int|r'|^2ds\right)^{1/2}
\leq\frac L{2\pi}\int|r'|^2ds=\frac{L^2}{2\pi}.
$$

If equality holds, the Wirtinger equalities give $r=p\cos(2\pi s/L)+q\sin(2\pi s/L)$. The arclength condition forces $|p|=|q|=L/(2\pi)$ and $p\cdot q=0$, so the boundary is a circle. A circle attains equality, making the constant optimal.

**The inequality and equality characterization persist for finitely many corners.** A rectifiable piecewise smooth simple closed curve has a Lipschitz arclength parametrization, with $|r'|=1$ almost everywhere. Green's theorem and the absolutely continuous version of Wirtinger's inequality used above still apply. More generally one may approximate a rectifiable Jordan curve by smooth curves while preserving the limiting length and area. If the allowed isolated singularities give infinite length, the inequality is trivially satisfied in the extended sense.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
