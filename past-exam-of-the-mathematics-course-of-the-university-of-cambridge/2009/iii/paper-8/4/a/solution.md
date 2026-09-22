<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The finite-dimensional [Krein-Milman theorem](../../../../../../krein-milman-theorem.md) says that a nonempty compact convex set $K$ is the [convex hull](../../../../../../convex-hull.md) of its [extreme points](../../../../../../extreme-point.md). A point is extreme if a proper convex combination of two points of $K$ equals it only when both points equal it.

Prove the theorem by induction on the dimension of the affine hull. Dimension zero is immediate. In positive dimension work inside that affine hull, where $K$ has interior. Every boundary point $x$ lies on a supporting hyperplane. To see this, choose exterior points $y_j\to x$ and nearest points $p_j\in K$. Convexity and the minimum-distance condition give $(y_j-p_j)\cdot(z-p_j)\leq0$ for $z\in K$. A subsequence of the normalized nonzero vectors $y_j-p_j$ converges to a unit vector $v$, while $p_j\to x$, giving $v\cdot(z-x)\leq0$. The resulting face $F=\{z\in K:v\cdot(z-x)=0\}$ has smaller affine dimension. Its [extreme points](../../../../../../extreme-point.md) are extreme in $K$, since equality in the supporting inequality forces both endpoints of any decomposition to lie in $F$. Induction expresses $x$ as a convex combination of [extreme points](../../../../../../extreme-point.md) of $K$.

Every interior point is a convex combination of the two endpoints of a line segment through it maximal in $K$; compactness gives the endpoints, and both are boundary points. Combining their convex decompositions completes the proof. In the generalization requested, a nonempty weak-star compact convex subset $K$ of the dual unit ball of a separable [Banach space](../../../../../../banach-space-split.md) satisfies

$$
\boxed{K=\overline{\operatorname{conv}(\operatorname{ext}K)}^{\,w^*}.}
$$

The closure is now essential; separability makes this compact weak-star setting metrizable but the general [Krein-Milman theorem](../../../../../../krein-milman-theorem.md) holds more broadly in locally convex spaces.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
