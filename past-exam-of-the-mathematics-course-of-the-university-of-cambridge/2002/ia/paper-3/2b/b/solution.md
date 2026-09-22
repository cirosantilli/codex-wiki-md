<h1 id="2b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Yes: every finite group of rotations about the origin in the plane is cyclic.** A [planar rotation](../../../../../../planar-rotation.md) is determined by an angle modulo $2\pi$, and composition adds those angles. If $G$ consists only of the identity, it is a [cyclic group](../../../../../../cyclic-group.md). Otherwise, finiteness allows us to choose the smallest positive representative angle $\alpha\in(0,2\pi)$ occurring in $G$.

Take any [planar rotation](../../../../../../planar-rotation.md) in $G$ with representative angle $\theta\in[0,2\pi)$. Write $\theta=q\alpha+r$, where $q$ is an integer and $0\leq r<\alpha$. The composition $R_\theta R_\alpha^{-q}$ belongs to $G$ and has angle $r$. Minimality of $\alpha$ forces $r=0$, so every element of $G$ is a power of $R_\alpha$.

Similarly, write $2\pi=m\alpha+r$ with $0\leq r<\alpha$. If $r>0$, the [planar rotation](../../../../../../planar-rotation.md) $R_\alpha^{-m}$ has representative angle $r$, a contradiction. Thus $\alpha=2\pi/m$ and

$$
\boxed{G=\langle R_{2\pi/m}\rangle.}
$$

This proves [finite groups of planar rotations are cyclic](../../../../../../finite-groups-of-planar-rotations-are-cyclic.md) by an elementary angle argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2B](../../2b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
