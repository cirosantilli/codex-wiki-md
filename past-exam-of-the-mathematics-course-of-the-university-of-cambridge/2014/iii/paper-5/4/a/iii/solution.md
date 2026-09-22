<h1 id="4/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the sharp [energy estimate](../../../../../../../energy-estimate.md), **$C_0=0$ stays uniform while the available bound $C_1=M^2/\varepsilon$ diverges as $\varepsilon\downarrow0$ when $M>0$.** If the coarser estimate is used for the first part, both displayed bounds $M^2/\varepsilon$ diverge, but the first divergence is only an artifact of discarding an exact cancellation.

The [method of characteristics](../../../../../../../method-of-characteristics.md) explains why uniform control of the [gradient](../../../../../../../gradient.md) cannot generally persist for the inviscid [scalar conservation law](../../../../../../../scalar-conservation-law.md). Before [characteristic crossing](../../../../../../../characteristic-crossing.md), with initial data $u_0$,

$$
x=\xi+tF'(u_0(\xi)),\qquad u(t,x)=u_0(\xi),\qquad
u_x(t,x)=\frac{u_0'(\xi)}{1+tF''(u_0(\xi))u_0'(\xi)}.
$$

If $F''(u_0(\xi))u_0'(\xi)<0$ somewhere, the denominator reaches zero in finite positive time. The solution steepens and the smooth description breaks down; an [entropy solution](../../../../../../../entropy-solution.md) can subsequently contain [shocks](../../../../../../../shock-wave.md). Positive viscosity replaces such a discontinuity by a thin smooth layer, which can have large [gradient](../../../../../../../gradient.md) even while its $L^2$ [norm](../../../../../../../norm.md) remains controlled. The divergent bound does not assert that every flux and every initial datum form a [shock](../../../../../../../shock-wave.md); a linear flux, for example, has no such steepening.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
