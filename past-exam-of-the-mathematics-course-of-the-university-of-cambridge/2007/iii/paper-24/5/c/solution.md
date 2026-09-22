<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $F\subseteq S^2_\infty$ be nonempty, closed and $\Gamma$-invariant. We first show it cannot be a singleton when $\Gamma$ is a [non-elementary Kleinian group](../../../../../../non-elementary-kleinian-group.md).

Suppose every element fixes one boundary point, conjugated to $\infty$. Each boundary map then has the affine form $z\mapsto az+b$. If all elements have $|a|=1$, their action in upper half-space keeps the height of $o$ fixed. An orbit sequence escaping compact interior sets must have its horizontal coordinate tending to infinity along any convergent boundary subsequence, so its only possible boundary limit is $\infty$. If some element has $|a|\ne1$, move its second fixed point to $0$, making it $f(z)=az$. For any $g(z)=cz+d$, its conjugates are $f^ngf^{-n}(z)=cz+a^nd$. Choose $n\to+\infty$ or $-\infty$ so $a^n\to0$. If $d\ne0$, these are distinct group elements converging to $z\mapsto cz$, contradicting discreteness. Thus $d=0$ for every group element: all fix both $0$ and $\infty$, and their only possible interior-orbit boundary limits are these two points. In both cases the [Kleinian limit set](../../../../../../limit-set-of-a-kleinian-group.md) has at most two points. This contradicts non-elementarity. Therefore $F$ has at least two distinct points.

Use the Klein ball model, in which hyperbolic geodesics are straight chords, and take the closed Euclidean convex hull $C$ of $F$ in the closed ball. It contains an interior point $o$, since the open chord between two distinct points of $F$ lies in the open ball. The interior part of this hull is hyperbolically convex and invariant under $\Gamma$: isometries preserve geodesic segments, so they preserve the hyperbolic convex hull of the invariant set. Thus $\Gamma o\subseteq C$.

The only points of $C$ on the boundary sphere are the points of $F$. Indeed, if $\xi\in S^2_\infty\setminus F$, [compactness](../../../../../../compact-space.md) of $F$ gives $\xi\cdot z\le c<1$ for every $z\in F$, because $\xi\cdot z=1$ on the unit sphere only when $z=\xi$. The same linear inequality holds throughout $C$, excluding $\xi$ from it. Conversely $F\subset C$, so $C\cap S^2_\infty=F$.

Every boundary accumulation point of $\Gamma o$ consequently lies in $F$. Base-point independence from part (b) identifies that accumulation set with $\Lambda(\Gamma)$, proving [minimality of the Kleinian limit set](../../../../../../minimality-of-the-kleinian-limit-set.md):

$$
\boxed{\Lambda(\Gamma)\subseteq F.}
$$

This proves the stated containment for every nonempty closed invariant set, not merely for sets containing an arbitrarily chosen orbit on the boundary.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
