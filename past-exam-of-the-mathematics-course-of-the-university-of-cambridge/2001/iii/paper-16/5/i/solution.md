<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First show that the [boundary](../../../../../../boundary-of-a-set.md) map is onto and has degree $\pm1$, and that the fundamental-group [injection](../../../../../../injective-function.md) is actually an [isomorphism](../../../../../../isomorphism.md). An [injective](../../../../../../injective-function.md) map between closed [surfaces](../../../../../../topological-surface.md) is a [homeomorphism](../../../../../../homeomorphism.md) onto an open-and-closed subset by [invariance of domain](../../../../../../invariance-of-domain.md). Thus each component of $\partial M$ maps homeomorphically to a distinct component of $\partial N$.

Orient $M$ and $N$, and write

$$
f_*[M,\partial M]=d[N,\partial N].
$$

Apply the [boundary](../../../../../../boundary-of-a-set.md) map in the relative [homology](../../../../../../homology-split.md) sequence. The [boundary](../../../../../../boundary-of-a-set.md) of the right side has coefficient $d$ on every [boundary](../../../../../../boundary-of-a-set.md) component of $N$. On the left, an image [boundary](../../../../../../boundary-of-a-set.md) component has coefficient $+1$ or $-1$, and an omitted component has coefficient zero. Since at least one component is present, $d=\pm1$; then no component can be omitted and all signs agree. Therefore

$$
\boxed{f|_{\partial M}:\partial M\longrightarrow\partial N\text{ is a homeomorphism},\qquad\deg f=\pm1.}
$$

Let $H=f_*\pi_1(M)$ and lift $f$ to the [connected](../../../../../../connected-space.md) cover $p:N_H\to N$ corresponding to $H$. If the cover were noncompact, then $H_3(N_H,\partial N_H;\mathbb Z)=0$. The lifted relative fundamental class would have zero [boundary](../../../../../../boundary-of-a-set.md), but its [boundary](../../../../../../boundary-of-a-set.md) is a nonzero sum of distinct [boundary](../../../../../../boundary-of-a-set.md) fundamental classes, since the original [boundary](../../../../../../boundary-of-a-set.md) map is [injective](../../../../../../injective-function.md) and the [boundary](../../../../../../boundary-of-a-set.md) components are [compact](../../../../../../compact-space.md). This is impossible. The cover therefore has a finite number $r$ of sheets. Degree multiplicativity gives

$$
\pm1=\deg f=r\,\deg\widetilde f.
$$

Hence $r=1$. The image of $f_*$ is the whole target [fundamental group](../../../../../../fundamental-group.md), and the assumed [injection](../../../../../../injective-function.md) makes **$f_*$ an [isomorphism](../../../../../../isomorphism.md)**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
