<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

In a [transformation model](../../../../../../transformation-model.md), a group acts on data $y$ and parameters compatibly: $Y\sim P_\theta$ implies $gY\sim P_{g\theta}$. A statistic $A$ is invariant if $A(gy)=A(y)$, and is a [maximal invariant](../../../../../../maximal-invariant.md) if equality of its values also implies the samples lie on the same group orbit. A maximal invariant records all information unchanged by the transformations; measurable invariant procedures therefore factor through it, subject to the ordinary orbit-space measurability conditions.

An [equivariant estimator](../../../../../../equivariant-estimator.md) satisfies $T(gy)=gT(y)$ for the induced action on the quantity estimated. For the positive affine location-scale group, $gy=a+by$ with $b>0$, this means $T_{\rm loc}(a+by)=a+bT_{\rm loc}(y)$ and $T_{\rm scale}(a+by)=bT_{\rm scale}(y)$.

For a nonconstant ordered sample, take $\bar y$ and $s^2=n^{-1}\sum_i(y_i-\bar y)^2>0$. Then

$$
A(y)=\left((y_i-\bar y)/s\right)_{i=1}^n
$$

is a [maximal invariant](../../../../../../maximal-invariant.md): it is unchanged by the positive affine group, and if $A(y)=A(z)$ then $z_i=\bar z+(s_z/s_y)(y_i-\bar y)$, explicitly recovering the transformation. Both mean and standard deviation are equivariant. If the whole model varies only by location and positive scale, the normalized sample's distribution is independent of those two parameters, giving an [ancillary statistic](../../../../../../ancillary-statistic.md). It may still retain information about additional shape parameters.

Equivariance yields a coherent transformation rule and, under an invariant loss, can simplify risk comparison to a reference parameter. It does not on its own establish optimality. Normalization by a parameter-space estimator with a nontrivial stabilizer requires quotienting that remaining action; otherwise an apparently standardized statistic need not be maximal.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
