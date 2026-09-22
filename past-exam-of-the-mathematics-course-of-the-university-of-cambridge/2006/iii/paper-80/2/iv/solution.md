<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $k=(a_1-a_0)/(a_1+2a_0)$. Far from all the small [spheres](../../../../../../sphere.md), their leading dipole contributions have the same direction and their leading $|x|^{-2}$ potential terms add:

$$
u(x)-x_3\simeq-k\left(\sum_jr_j^3\right)\frac{x_3}{|x|^3}.
$$

Translations of their centres change only higher far-field multipoles. Since the outer body is a [sphere](../../../../../../sphere.md) of radius $R_0$,

$$
p=\frac{\sum_jr_j^3}{R_0^3}.
$$

Replacing the whole body by an [isotropic](../../../../../../isotropy.md) effective [sphere](../../../../../../sphere.md) of conductivity $a^*$ gives its leading dipole coefficient $R_0^3(a^*-a_0)/(a^*+2a_0)$. Matching coefficients yields

$$
\frac{a^*-a_0}{a^*+2a_0}=pk.
$$

Solving this equation gives the [Maxwell approximation for conductivity](../../../../../../maxwell-approximation-for-conductivity.md):

$$
\boxed{
a^*=a_0\frac{1+2pk}{1-pk}
=a_0+\frac{3pa_0(a_1-a_0)}{3a_0+(1-p)(a_1-a_0)}.
}
$$

For positive phase conductivities and $0\le p\le1$, the denominator is positive. This rational approximation is obtained by dipole matching; its extrapolation beyond the dilute regime is a closure assumption, not an exact formula for arbitrary inclusion arrangements.

For the consistency check, $\beta=3a_0k$, so its dilute expansion is

$$
a^*=a_0+\frac{p\beta}{1-p\beta/(3a_0)}
=a_0+p\beta+\frac{p^2\beta^2}{3a_0}+O(p^3).
$$

The [isotropic](../../../../../../isotropy.md) interaction relation supplied in part (iii) gives

$$
a^*\simeq a_0I+p\beta I-\beta^2\left(-\frac{p^2}{3a_0}I\right)
=\left(a_0+p\beta+\frac{p^2\beta^2}{3a_0}\right)I.
$$

Thus **the Maxwell approximation and the interaction correction agree through second order in [volume fraction](../../../../../../volume-fraction.md)**.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
