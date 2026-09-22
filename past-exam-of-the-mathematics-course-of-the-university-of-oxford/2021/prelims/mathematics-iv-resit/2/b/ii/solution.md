<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A possible center $\mathbf c$ must be a [fixed point](../../../../../../../fixed-point.md), so $(I-R_\theta)\mathbf c=\mathbf b$. Let $c=\cos\theta$ and $s=\sin\theta$. The [determinant](../../../../../../../determinant.md) is

$$
\det(I-R_\theta)=(1-c)^2+s^2=2(1-c)=4\sin^2(\theta/2)>0
$$

when $\theta$ is not an [integer multiple](../../../../../../../integer-multiple.md) of $2\pi$. The unique center is therefore

$$
\boxed{\mathbf c=(I-R_\theta)^{-1}\mathbf b=\frac1{2(1-\cos\theta)}\begin{pmatrix}1-\cos\theta&-\sin\theta\\\sin\theta&1-\cos\theta\end{pmatrix}\mathbf b.}
$$

The [fixed point](../../../../../../../fixed-point.md) equation implies $\mathbf b=\mathbf c-R_\theta\mathbf c$, whence

$$
T(\mathbf v)=\mathbf c+R_\theta(\mathbf v-\mathbf c).
$$

Relative to $\mathbf c$, this is precisely a [planar rotation](../../../../../../../planar-rotation.md) through $\theta$. This also explains the excluded case: when $\theta\in2\pi\mathbb Z$, $T$ is a [translation](../../../../../../../translation-geometry.md), with no [fixed point](../../../../../../../fixed-point.md) unless $\mathbf b=0$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Mathematics IV resit](../../../../mathematics-iv-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
