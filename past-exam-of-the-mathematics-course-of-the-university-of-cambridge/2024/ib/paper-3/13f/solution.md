<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

For a closed piecewise [smooth curve](../../../../../smooth-curve.md) $\gamma$ avoiding $w$, its [winding number](../../../../../winding-number.md) about $w$ is

$$
\boxed{
\operatorname{wind}(\gamma,w)
=\frac1{2\pi i}\int_\gamma\frac{dz}{z-w}}.
$$

The [argument principle](../../../../../argument-principle.md) says that if a positively oriented closed curve $\gamma$ bounds a domain $U$, and a meromorphic [function](../../../../../function-split.md) $F$ has no zeros or poles on $\gamma$, then

$$
\boxed{
\frac1{2\pi i}\int_\gamma\frac{F'(z)}{F(z)}\,dz
=N_U(F)-P_U(F)},
$$

where zeros and poles are counted with multiplicity.

Suppose $F$ and $G$ are holomorphic on a neighbourhood of $\overline U$ and

$$
|G(z)|<|F(z)|
\qquad(z\in\gamma).
$$

For $0\leq t\leq1$, $F+tG$ has no boundary zero, because a zero would imply $|F|=t|G|<|F|$. Its argument-principle count is integer-valued and continuous in $t$, hence constant. Thus [Rouché's theorem](../../../../../rouche-s-theorem.md) states that

$$
\boxed{F\text{ and }F+G\text{ have the same number of zeros in }U}.
$$

Now let $w_0=f(z_0)$. Since $|w_0|<1\leq|f|$ on the unit circle, Rouché's theorem shows that $f$ and $f-w_0$ have the same number of zeros in the unit disc. The latter has the zero $z_0$, so $f$ has at least one zero there. For any $w$ with $|w|<1$, the same boundary inequality shows that $f-w$ has the same positive number of zeros as $f$. Therefore

$$
\boxed{\mathbb D\subseteq f(\mathbb D)}.
$$

This is the [unit-disc image from a boundary modulus lower bound](../../../../../unit-disc-image-from-a-boundary-modulus-lower-bound.md).

Finally, take a sufficiently small positively oriented circle $C$ around zero. The residue

$$
k=\operatorname{res}_{0}\frac{g'}g
=\frac1{2\pi i}\int_C\frac{g'}g\,dz
$$

is the winding number of $g(C)$ around zero, so $k\in\mathbb Z$. The pole is simple, hence its residue is nonzero and $k\ne0$. For

$$
h(z)=z^{-k}g(z)
$$

we have

$$
\frac{h'}h=\frac{g'}g-\frac{k}{z}.
$$

The second term cancels the complete principal part at zero, so the [integer residue of a logarithmic derivative](../../../../../integer-residue-of-a-logarithmic-derivative.md) proves that $h'/h$ has a removable singularity there.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
