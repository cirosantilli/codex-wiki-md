<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [orientable surface](../../../../orientable-surface.md) admits local coordinate orientations that are consistent on overlaps. Equivalently a [triangulation](../../../../triangulation.md) can be oriented so that adjacent faces induce opposite directions on their common edge. Use a polygon word to record its successive boundary edges, identifying equal letters in their indicated directions; a negative exponent reverses that edge direction.

Square models are **$P:abab$, $K:aba^{-1}b$, and $T:aba^{-1}b^{-1}$**. The first identifies antipodal boundary points of a disk, giving the [real projective plane](../../../../real-projective-plane.md). Only the [torus](../../../../torus.md) among these three is [orientable](../../../../orientable-surface.md): its paired sides traverse the boundary oppositely, whereas each other model has a same-direction pair. The projective model has two vertex classes, and the other two one, giving Euler characteristics one and zero respectively.

The other possibility is **the [sphere](../../../../sphere.md)**, for example the word $aa^{-1}bb^{-1}$ with three vertex classes. There are no others: a paired square has one face, two edges and between one and three vertex classes, so its [Euler characteristic](../../../../euler-characteristic.md) is $V-1\in\{0,1,2\}$. The [classification of compact surfaces](../../../../classification-of-compact-surfaces.md) leaves precisely the [sphere](../../../../sphere.md), [real projective plane](../../../../real-projective-plane.md), [torus](../../../../torus.md) and [Klein bottle](../../../../klein-bottle.md) at those values, with the indicated orientabilities.

For connected sums, remove a disk from each [surface](../../../../topological-surface-split.md), join the resulting boundary circles, and cut a joining arc to produce a single polygon. Its word concatenates the two original words. The [real projective plane](../../../../real-projective-plane.md) also has the bigon word $cc$, so

$$
\boxed{T\mathbin{\#}P:\ aba^{-1}b^{-1}cc,\qquad T\mathbin{\#}K:\ aba^{-1}b^{-1}cdc^{-1}d.}
$$

These use respectively six and eight sides, proving the requested hexagon and octagon constructions. Their Euler characteristics are $-1$ and $-2$, also obtained from $\chi(X\#Y)=\chi(X)+\chi(Y)-2$.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the geometry course of the University of Oxford](../../../split.md)
5. [Geometry course of the University of Oxford](../../../../geometry-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
