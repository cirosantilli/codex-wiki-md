<h1 id="e/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Hausdorff space](../../../../hausdorff-space.md) separates any two distinct points by disjoint [open neighborhoods](../../../../open-neighbourhood.md). For a subspace $A\subseteq X$, intersect such neighborhoods in $X$ with $A$ to obtain disjoint neighborhoods in the [subspace topology](../../../../subspace-topology.md). Thus subspaces inherit the [Hausdorff](../../../../hausdorff-space.md) property.

If $(z_1,z_2)$ lies off the diagonal of a [Hausdorff space](../../../../hausdorff-space.md)'s square, choose disjoint [open neighborhoods](../../../../open-neighbourhood.md) $U$ of $z_1$ and $V$ of $z_2$. The [open](../../../../open-set.md) rectangle $U\times V$ contains the pair and avoids the diagonal. Therefore its complement is [open](../../../../open-set.md) and the diagonal is [closed](../../../../closed-set.md).

The map $F:X\times Y\to Z\times Z$ given by $F(x,y)=(f(x),g(y))$ is [continuous](../../../../continuous-function.md) by the coordinate criterion from E3. The equality locus is $F^{-1}(\Delta_Z)$ and is [closed](../../../../closed-set.md) as an [inverse image](../../../../preimage.md) of a [closed set](../../../../closed-set.md).

Let $q:X\to X/{\sim}$ be the [quotient map](../../../../quotient-map.md). If the [quotient](../../../../quotient.md) is [Hausdorff](../../../../hausdorff-space.md), apply the same argument to $q$ in both coordinates:

$$
R=(q\times q)^{-1}(\Delta_{X/{\sim}})
$$

is [closed](../../../../closed-set.md) in $X\times X$.

Conversely suppose $R$ is [closed](../../../../closed-set.md) and $q$ is [open](../../../../open-set.md). Take two distinct [quotient](../../../../quotient.md) points, with representatives $x,y$. Since $(x,y)\notin R$, an [open](../../../../open-set.md) rectangle $U\times V$ around it avoids $R$. The [images](../../../../image-of-a-function.md) $q(U)$ and $q(V)$ are [open](../../../../open-set.md) [quotient](../../../../quotient.md) neighborhoods. They are disjoint, because a [quotient](../../../../quotient.md) point in their [intersection](../../../../set-intersection.md) would have equivalent representatives $u\in U$, $v\in V$, giving $(u,v)\in R$. Hence the [quotient](../../../../quotient.md) is [Hausdorff](../../../../hausdorff-space.md). Thus **closedness of the relation and openness of the [quotient map](../../../../quotient-map.md) suffice for a [Hausdorff](../../../../hausdorff-space.md) [quotient](../../../../quotient.md)**.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [E](../../e.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
