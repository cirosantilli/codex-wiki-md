<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $M$ for either [connected](../../../../../connected-space.md) closed oriented [manifold](../../../../../topological-manifold-split.md) and $D$ for its embedded closed ball. A precise relative form of [Poincare duality](../../../../../poincare-duality.md) for a compact locally contractible subset is

$$
H_j(M,M\setminus D;\mathbb Z)\cong H^{n-j}(D;\mathbb Z).
$$

This is [Poincaré-Alexander duality](../../../../../poincare-alexander-duality.md). It applies to the printed closed-ball complement without replacing $D$ by its interior. Since $D$ is contractible, the relative group is $\mathbb Z$ at $j=n$ and zero otherwise. Naturality identifies $H_n(M)\to H_n(M,M\setminus D)$ with restriction $H^0(M)\to H^0(D)$, which is an [isomorphism](../../../../../isomorphism.md) because both spaces are [connected](../../../../../connected-space.md). Equivalently, the [fundamental class](../../../../../fundamental-class.md) restricts to the relative [orientation](../../../../../orientation-of-a-simplex.md) generator on the ball.

In the [long exact sequence of a pair](../../../../../long-exact-sequence-in-relative-homology.md), the only potentially exceptional part is therefore

$$
0\to H_n(M\setminus D)\to H_n(M)\xrightarrow{\cong}\mathbb Z
\to H_{n-1}(M\setminus D)\to H_{n-1}(M)\to0.
$$

Exactness gives $H_n(M\setminus D)=0$ and the desired [isomorphism](../../../../../isomorphism.md) in degree $n-1$. In every lower degree both adjacent relative terms are zero, so the same exact sequence gives the remaining isomorphisms. Thus

$$
\boxed{H_k(M_i\setminus D_i)\cong H_k(M_i),\qquad0\leq k<n}.
$$

For the pieces $M_i\setminus\operatorname{int}D_i$ used in the gluing, the same conclusion follows from [excision](../../../../../excision-theorem.md) and the pair $(D^n,S^{n-1})$, or from the radial deformation of a punctured ball to its boundary. These pieces also have zero top homology, and the image of their boundary [sphere](../../../../../sphere.md)'s [fundamental class](../../../../../fundamental-class.md) is zero: it is the boundary of their relative oriented fundamental chain.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../../split.md)
6. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
