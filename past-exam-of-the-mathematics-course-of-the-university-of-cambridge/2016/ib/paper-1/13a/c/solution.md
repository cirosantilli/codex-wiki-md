<h1 id="13a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the parabolic domain with the nonpositive real axis removed, first apply the [principal square root](../../../../../../principal-square-root-of-a-complex-number.md), then scale by $\pi/2$, and then apply the map of part (b). This gives the stated composite $C(z)$ and maps bijectively onto the slit [unit disc](../../../../../../unit-disc.md).

There is no genuine [branch cut](../../../../../../branch-cut.md) in the composite. The function $\tan^2(\pi s/4)$ is even in $s$, so changing the local square root has no effect. Near zero its [Taylor series](../../../../../../taylor-series.md) starts as

$$
\tan^2(\pi\sqrt z/4)=\frac{\pi^2}{16}z+O(z^2),
$$

giving a [holomorphic](../../../../../../complex-differentiability-at-a-point.md) extension with $C(0)=0$. There are no [poles](../../../../../../pole.md) within the parabolic domain: the possible squared locations are $z=(2+4k)^2$, all on the excluded real portion $x\geq4$.

For $z=-r^2$ with $r\geq0$, the continuation gives

$$
C(-r^2)=-\tanh^2(\pi r/4).
$$

As $r$ ranges from zero to infinity, these values run once through $(-1,0]$. They fill precisely the slit omitted by the previous mapping, and no point away from the negative real axis has an image in that slit. Therefore **the extended map is a bijection onto the whole unit disc**:

$$
\boxed{C:\{x+iy:y^2<4(1-x)\}\longrightarrow\{w:|w|<1\}.}
$$

It is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) throughout, so this bijection is the desired [conformal map from a parabolic domain to the unit disc](../../../../../../conformal-map-from-a-parabolic-domain-to-the-unit-disc.md); in particular $C'(0)=\pi^2/16\ne0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13A](../../13a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
