<h1 id="20f/solution">Solution</h1>

↑ **Parent:** [20F](../20f.md)

Let $q:S^2\to X$ identify the two points to $p$. Take disjoint small open disks around the original points and let $U$ be their image; $U$ is a contractible wedge of two disks. Let $V=X\setminus\{p\}$, which is homeomorphic to a sphere with two punctures and retracts onto a circle. Then $U\cap V$ consists of two punctured disks, each retracting onto a circle.

In the [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md), the map $H_1(U\cap V)=\mathbb Z^2\to H_1(U)\oplus H_1(V)=\mathbb Z$ has rank one and is surjective: both annular loops map to generators, with a possible orientation sign. Its kernel is $\mathbb Z$, so $H_2(X)=\mathbb Z$. At degree zero the map $\mathbb Z^2\to\mathbb Z\oplus\mathbb Z$ is $(a,b)\mapsto(a+b,-a-b)$, with rank-one kernel. The preceding degree-one map is surjective, so exactness gives $H_1(X)=\mathbb Z$. Since $X$ is connected and both pieces have no higher homology,

$$
\boxed{H_j(X;\mathbb Z)=\begin{cases}\mathbb Z,&j=0,1,2,\\0,&j\geq3.\end{cases}\qquad b_0=b_1=b_2=1.}
$$

This illustrates [homology after identifying two points on a sphere](../../../../../homology-after-identifying-two-points-on-a-sphere.md).

## ↑ Ancestors (10)

1. [20F](../20f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
