<h1 id="a/3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[No slip](../../../../../no-slip-boundary-condition.md) on the two fixed radial walls gives $g(\pm\alpha)=0$. The outward [flux](../../../../../flux.md) through a circular arc is $\int_{-\alpha}^\alpha u_r r\,d\theta=\int_{-\alpha}^\alpha g\,d\theta$, so [source strength](../../../../../volumetric-flow-rate.md) $Q$ requires that integral to equal $Q$. Set $g=QG$ and $\epsilon=Q/\nu$. Then

$$
G^{(3)}+4G'+2\epsilon GG'=0,\quad G(\pm\alpha)=0,\quad\int_{-\alpha}^\alpha G\,d\theta=1.
$$

At leading order $G_0^{(3)}+4G_0'=0$, whose general solution is a constant plus sine and cosine of $2\theta$. The symmetric source-driven branch has no sine term; for generic $\alpha$ this also follows directly by subtracting its two wall conditions. Thus

$$
\boxed{G_0=C(\cos2\theta-\cos2\alpha),\qquad C=\frac1{\sin2\alpha-2\alpha\cos2\alpha}.}
$$

Indeed its integral is $C(\sin2\alpha-2\alpha\cos2\alpha)=1$. At isolated angles where an odd zero-[flux](../../../../../flux.md) homogeneous mode satisfies both wall conditions, symmetry selects the stated branch.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
