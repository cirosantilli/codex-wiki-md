<h1 id="5e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $v=x-a$ and decompose it into axial and perpendicular parts, $v=(v\cdot n)n+v_\perp$. For the nondegenerate semi-angle $0<\alpha<\pi/2$, the equation is equivalent to

$$
|v_\perp|^2\cos^2\alpha=(v\cdot n)^2\sin^2\alpha,\qquad |v_\perp|=|v\cdot n|\tan\alpha.
$$

Thus each plane perpendicular to $n$ at axial distance $s$ from $a$ meets the surface in a circle of radius $|s|\tan\alpha$. Both signs of $s$ are allowed, and $s=0$ gives the vertex. This proves that it is a [double circular cone](../../../../../../double-circular-cone.md) with the specified vertex and axis; $\alpha$ is the angle each generator makes with either direction of the axis.

For the intersection calculation, define the symmetric [matrix](../../../../../../matrix.md) $Q=\cos^2\alpha\,I-nn^T$. The two equations are $(x-a_i)^TQ(x-a_i)=0$. Their difference gives

$$
-2x\cdot Q(a_1-a_2)+a_1\cdot Qa_1-a_2\cdot Qa_2=0.
$$

With $b=a_1-a_2$ and $m=(a_1+a_2)/2$, symmetry of $Q$ makes the last two terms $2m\cdot Qb$. Hence the [intersection plane of parallel congruent double cones](../../../../../../intersection-plane-of-parallel-congruent-double-cones.md) is

$$
\boxed{(Qb)\cdot(x-m)=0}.
$$

The unnormalized [normal vector](../../../../../../normal-vector.md) is $v=Qb=b\cos^2\alpha-n(n\cdot b)$. Expanding its squared norm gives

$$
|v|^2=|b|^2\cos^4\alpha+(n\cdot b)^2(1-2\cos^2\alpha).
$$

Equivalently, if $b=b_\perp+(n\cdot b)n$, this is $\cos^4\alpha|b_\perp|^2+\sin^4\alpha(n\cdot b)^2>0$. Thus normalization is legitimate and yields

$$
\boxed{N=\frac{b\cos^2\alpha-n(n\cdot b)}{\sqrt{|b|^2\cos^4\alpha+(n\cdot b)^2(1-2\cos^2\alpha)}}}.
$$

The assumption of a genuine cone matters: at the degenerate limits $\alpha=0$ or $\pi/2$, the surface collapses respectively to an axis or a plane and this normal need not exist.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5E](../../5e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
