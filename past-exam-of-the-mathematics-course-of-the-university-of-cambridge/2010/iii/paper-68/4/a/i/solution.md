<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $U$ be real and twice continuously differentiable, take a nonzero real [wave number](../../../../../../../wavenumber.md), and write $c=c_r+ic_i$. Exponential instability requires $kc_i>0$, in particular $c_i\ne0$, so $U-c$ has no zero on the channel. Divide the [Rayleigh equation for inviscid shear flow](../../../../../../../rayleigh-equation-for-inviscid-shear-flow.md) by $U-c$, multiply by $\psi^*$ and integrate. The wall conditions remove the boundary term, giving

$$
I+\int_{y_1}^{y_2}\frac{U''}{U-c}|\psi|^2dy=0,\qquad I=\int_{y_1}^{y_2}(|\psi'|^2+k^2|\psi|^2)dy>0.
$$

Its imaginary part is

$$
c_i\int_{y_1}^{y_2}\frac{U''|\psi|^2}{(U-c_r)^2+c_i^2}\,dy=0.
$$

The weight is nonnegative and positive wherever the nontrivial [eigenfunction](../../../../../../../eigenfunction.md) does not vanish. A nontrivial solution of this regular second-order equation cannot vanish on an interval. If $U''$ had one strict sign without changing sign, the [integral](../../../../../../../integral.md) could not vanish. If $U''$ were identically zero, the real identity would instead give the contradiction $I=0$. Thus $U''$ must take both signs, and continuity gives an interior zero. This proves **[Rayleigh's inflection-point theorem](../../../../../../../rayleigh-s-inflection-point-theorem.md): an unstable profile must have an [inflection point](../../../../../../../inflection-point.md)**, in fact a sign change of $U''$ rather than merely an isolated zero without sign change.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 68](../../../../paper-68-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
