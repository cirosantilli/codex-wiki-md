<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Using the first [partial derivatives](../../../../../../partial-derivative.md) from part (b),

$$
vg_u-ug_v=2uvf_x+(v^2-u^2)f_y=2yf_x-2xf_y.
$$

Also $uvg=yf$. Therefore the first [partial differential equation](../../../../../../partial-differential-equation-split.md) becomes

$$
\boxed{2y\frac{\partial f}{\partial x}-2x\frac{\partial f}{\partial y}+yf=0.}
$$

For the second [partial differential equation](../../../../../../partial-differential-equation-split.md), the same [chain rule](../../../../../../chain-rule.md) gives

$$
ug_u-vg_v=(u^2+v^2)f_x,\qquad (u^4-v^4)g=2x(u^2+v^2)f.
$$

Away from the origin, cancellation yields $f_x+2xf=0$. Treating $y$ as fixed, an [integrating factor](../../../../../../integrating-factor.md) gives $\partial_x(e^{x^2}f)=0$. Thus

$$
\boxed{f(x,y)=e^{-x^2}F(y),}
$$

where $F$ is an arbitrary sufficiently [differentiable function](../../../../../../differentiable-function.md). This is the local [general solution](../../../../../../general-solution.md), and the global form when $f$ is defined on the whole plane. If $f$ and its first [partial derivatives](../../../../../../partial-derivative.md) are continuous at the origin, the reduced [partial differential equation](../../../../../../partial-differential-equation-split.md) also holds there by [continuity](../../../../../../continuous-function.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
