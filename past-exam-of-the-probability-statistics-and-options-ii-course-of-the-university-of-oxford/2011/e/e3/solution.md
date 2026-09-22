<h1 id="e/e3/solution">Solution</h1>

↑ **Parent:** [E3](../e3.md)

A [connected space](../../../../connected-space.md) has no separation into two disjoint nonempty open subsets whose union is the space. A continuous surjection to the discrete space $\{0,1\}$ produces such a separation by the two point preimages. Conversely, from a separation define a function equal to zero on one open piece and one on the other; it is continuous and surjective. Thus these formulations of [connectedness](../../../../connected-space.md) are equivalent.

An interval in $\mathbb R$ is connected: if a continuous map from it to $\{0,1\}$ took both values, the intermediate value theorem would force value $1/2$, impossible. Conversely, a subset of $\mathbb R$ that is not an interval has points $a<b$ in it and a point $c\in(a,b)$ outside it. Intersecting it with $(-\infty,c)$ and $(c,\infty)$ separates it. The empty set is connected, and singleton intervals are included.

For the union assertion, any separation of $X$ must put each nonempty connected $A_i$ entirely on one side, since intersecting the separation with $A_i$ would otherwise disconnect it. Pairwise nonempty intersections force all the $A_i$ onto the same side. Their union is $X$, contradicting a nonempty second side. The empty-union case is already connected.

The plane is the union of all lines through the origin. Each line is homeomorphic to $\mathbb R$ and connected, and every pair meets at the origin, so $\mathbb R^2$ is connected. For the punctured plane, let $R_+$ be the positive horizontal ray, and for each $r>0$ let $C_r$ be the circle of radius $r$. Each circle is a continuous image of $[0,2\pi]$ and hence connected; $C_r\cup R_+$ is connected because its two connected pieces meet at $(r,0)$. These unions all contain $R_+$ and cover the punctured plane, proving it connected as well.

Finally suppose a continuous injection $g:\mathbb R^2\to\mathbb R$ existed. Its image is a connected interval, since a continuous image of a [connected space](../../../../connected-space.md) is connected. It contains at least three distinct values; choose $p$ whose value lies strictly between two others. The punctured plane $\mathbb R^2\setminus\{p\}$ is connected by translation of the preceding result. By injectivity its image is precisely $g(\mathbb R^2)\setminus\{g(p)\}$, which is disconnected by the missing interior point. This contradicts [connectedness](../../../../connected-space.md) of a continuous image. Therefore

$$
\boxed{\text{There is no continuous injection }\mathbb R^2\to\mathbb R.}
$$

## ↑ Ancestors (12)

1. [E3](../e3.md)
2. [E](../../e.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
