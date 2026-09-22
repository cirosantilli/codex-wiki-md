<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $q^2=k^2+l^2$ and $c=c_r+ic_i$, with $k>0$ chosen for the temporal mode convention. In the [inviscid limit](../../../../../../../euler-limit.md), the [Orr-Sommerfeld equation](../../../../../../../orr-sommerfeld-equation.md) reduces to the [Rayleigh equation for inviscid shear flow](../../../../../../../rayleigh-equation-for-inviscid-shear-flow.md):

$$
v''-q^2v-\frac{U''}{U-c}v=0.
$$

The impermeability [boundary condition](../../../../../../../boundary-condition.md) is $v(\pm1)=0$; the extra viscous derivative condition is not an independent condition for this reduced second-order equation. For an unstable mode $c_i>0$, the denominator has no real zero. Multiply by $\bar v$ and apply [integration by parts](../../../../../../../integration-by-parts.md) to obtain

$$
\int_{-1}^{1}(|v'|^2+q^2|v|^2)\,dy+\int_{-1}^{1}\frac{U''(U-c_r+ic_i)}{|U-c|^2}|v|^2\,dy=0.
$$

Its imaginary part gives

$$
\boxed{c_i\int_{-1}^{1}\frac{U''|v|^2}{|U-c|^2}\,dy=0.}
$$

For a nontrivial mode, the weight is nonnegative and is positive except at isolated mode zeros. Thus $U''$ must take both signs, unless it vanishes identically. The identically zero case also has no unstable nontrivial mode, by the positive first integral in the displayed identity. Therefore the smooth real base-flow profile must have an interior [inflection point](../../../../../../../inflection-point.md). This proves [Rayleigh's inflection-point theorem](../../../../../../../rayleigh-s-inflection-point-theorem.md); it is a necessary condition, not a sufficiency test.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 79](../../../../paper-79-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
