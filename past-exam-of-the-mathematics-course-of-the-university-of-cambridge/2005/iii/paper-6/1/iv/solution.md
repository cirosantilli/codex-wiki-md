<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The real space $C(\mathbb T)$ is a [Banach space](../../../../../../banach-space-split.md) in the [uniform norm](../../../../../../supremum-norm.md): a uniformly [Cauchy sequence](../../../../../../cauchy-sequence.md) has a uniform pointwise limit by [completeness](../../../../../../completeness.md) of $\mathbb R$, and that [uniform limit](../../../../../../uniform-limit.md) is [continuous](../../../../../../continuous-function.md). Each functional $L_N$ from the preceding part is bounded, but their norms are unbounded.

For integers $m\geq1$, define

$$
E_m=\{f\in C(\mathbb T):|L_Nf|\leq m\text{ for every }N\}.
$$

Each $E_m$ is [closed](../../../../../../closed-set.md), being an intersection of inverse images of [closed](../../../../../../closed-set.md) intervals under [continuous](../../../../../../continuous-function.md) functionals. It has empty interior. Otherwise some ball $B(f_0,r)$ would be contained in it. For every $h$ of [norm](../../../../../../norm.md) at most one, both $f_0$ and $f_0+(r/2)h$ would belong to that ball, so

$$
\frac r2|L_Nh|\leq |L_N(f_0+(r/2)h)|+|L_Nf_0|\leq2m.
$$

Taking the [supremum](../../../../../../supremum.md) over $h$ would give $\|L_N\|\leq4m/r$ for all $N$, contradicting the preceding part.

Thus the $E_m$ are [nowhere dense](../../../../../../nowhere-dense-set.md). The [Baire category theorem](../../../../../../baire-category-theorem.md) says their union cannot cover $C(\mathbb T)$. A function outside that union satisfies

$$
\boxed{\sup_N|S_N(f,0)|=\infty,}
$$

so its [Fourier series](../../../../../../fourier-series-split.md) diverges at zero. In fact these functions form a [dense](../../../../../../dense-set.md) $G_\delta$ subset of $C(\mathbb T)$. This proves the relevant [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) argument directly and establishes [generic unbounded Fourier sums at a fixed point](../../../../../../generic-unbounded-fourier-sums-at-a-fixed-point.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
