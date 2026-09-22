<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the construction, use the standard basic-sequence selection procedure. At stage $n$, choose finitely many functionals which almost norm the unit sphere of the finite-dimensional span of the vectors already chosen. Put the next vector in their common kernels, and in the analogous kernels retained from earlier stages. These impose only finite codimension. Choosing the norming tolerances with a finite product gives a uniformly bounded [basis constant](../../../../../../basis-constant.md), which may be fixed in advance, for example below two. The hypothesis then supplies a unit vector in this finite-codimensional subspace with image smaller than the prescribed $\varepsilon_n$. This yields the requested normalized [basic sequence](../../../../../../basic-sequence.md).

For strict singularity, fix $\eta>0$ and make the construction with a summable sequence satisfying $2K\sum_n\varepsilon_n<\eta$, where $K$ is the controlled [basis constant](../../../../../../basis-constant.md). For $z=\sum a_ne_n$, the coordinate bound $|a_n|\leq2K\|z\|$ gives

$$
\|Tz\|\leq\sum|a_n|\|Te_n\|\leq2K\sum\varepsilon_n\,\|z\|<\eta\|z\|.
$$

By density this holds on the infinite-dimensional closed span $E$.

If $T$ were bounded below by $c>0$ on some infinite-dimensional subspace $Y$, choose $\eta<c/2$. Hereditary indecomposability supplies unit vectors $y\in Y,e\in E$ arbitrarily close. Then

$$
c\leq\|Ty\|\leq\|Te\|+\|T\|\|y-e\|<c/2+\|T\|\|y-e\|,
$$

a contradiction for sufficiently close vectors. Therefore **$T$ is a strictly singular operator**, equivalently every infinite-dimensional subspace contains a unit vector with arbitrarily small image. The case $T=0$ is immediate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
