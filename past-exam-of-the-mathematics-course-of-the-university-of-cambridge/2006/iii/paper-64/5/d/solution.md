<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The imaginary [quaternions](../../../../../../quaternion.md) form Euclidean $\mathbb R^3$. Conjugation by a [unit quaternion](../../../../../../unit-quaternion.md) acts by

$$
v\longmapsto qvq^{-1}.
$$

It preserves the imaginary subspace and its [norm](../../../../../../norm.md), and continuity from $q=1$ gives [determinant](../../../../../../determinant.md) $+1$. The kernel consists of [quaternions](../../../../../../quaternion.md) commuting with all imaginary [quaternions](../../../../../../quaternion.md), hence is $\{\pm1\}$.

For a unit imaginary [quaternion](../../../../../../quaternion.md) $n$, take $q=\cos(\theta/2)+n\sin(\theta/2)$. If $v$ is perpendicular to $n$, [quaternion](../../../../../../quaternion.md) multiplication gives

$$
qvq^{-1}=v\cos\theta+(n\times v)\sin\theta,
$$

while the component parallel to $n$ is unchanged. This produces the rotation through angle $\theta$ about axis $n$, and every element of $SO(3)$ has such an axis-angle description. The map is surjective, yielding

$$
\boxed{SO(3)\cong SU(2)/\{\pm I\}.}
$$

The half-angle also explains why $q$ and $-q$ give the same rotation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
