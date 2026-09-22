<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use a [gravity-current box model](../../../../../../gravity-current-box-model.md): approximate the current by uniform depth $h(t)$ and length $L(t)$, with constant [reduced gravity](../../../../../../reduced-gravity-split.md), no deposition and no [fluid entrainment](../../../../../../fluid-entrainment.md). The triangular cross-sectional area is $h^2/2$, so the fixed released volume is

$$
V_0=\frac12Lh^2,\qquad h=\left(\frac{2V_0}{L}\right)^{1/2}.
$$

The [Benjamin deep-ambient front condition](../../../../../../benjamin-deep-ambient-front-condition.md) closes the integral model:

$$
\dot L=\sqrt{2g'h}=F\sqrt{g'}(2V_0)^{1/4}L^{-1/4},\qquad F=\sqrt2.
$$

For a finite initial length $L_0$, direct [integration](../../../../../../integral.md) gives

$$
\boxed{L(t)=\left[L_0^{5/4}+\frac54F\sqrt{g'}(2V_0)^{1/4}t\right]^{4/5},\qquad h(t)=\sqrt{2V_0/L(t)}.}
$$

The ideal point-release limit takes $L_0=0$ and has $L\propto t^{4/5}$, $h\propto t^{-2/5}$. Its divergent initial depth is outside the [shallow water](../../../../../../shallow-water-approximation.md) approximation, so a real finite reservoir regularizes the early stage. This is the [finite-volume triangular-channel current](../../../../../../finite-volume-triangular-channel-current.md) integral law; it does not assert a spatially uniform exact solution of the local equations.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Section B](../../section-b.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
