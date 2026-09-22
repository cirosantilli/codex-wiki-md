<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

Label the edges so that barycentric coordinates on $T$ satisfy

$$
I=\{u=0\},\qquad J=\{v=0\},\qquad K=\{w=0\},
\qquad u+v+w=1.
$$

Suppose for contradiction that $A\cap B\cap C=\varnothing$. The [distance from a point to a closed set](../../../../../distance-from-a-point-to-a-closed-set.md) gives continuous nonnegative functions $d_A,d_B,d_C$. Their sum never vanishes, while at every point at least one of them vanishes because $A\cup B\cup C=T$. Hence

$$
F(x)=\frac{(d_A(x),d_B(x),d_C(x))}
{d_A(x)+d_B(x)+d_C(x)}
$$

is a continuous map from $T$ to its boundary in barycentric-coordinate space. Moreover, $F(I)\subseteq I$, $F(J)\subseteq J$, and $F(K)\subseteq K$. On each edge, the straight-line homotopy between $F$ and the identity remains in that edge, so $F|_{\partial T}$ has [winding number](../../../../../winding-number.md) one. On the other hand, a map from the whole triangle to its boundary makes its boundary restriction [null-homotopic](../../../../../null-homotopic-map.md), and hence gives winding number zero. This contradiction proves the three-set covering lemma:

$$
\boxed{A\cap B\cap C\ne\varnothing}.
$$

If a [retraction](../../../../../retraction.md) $f:D\to\partial D$ fixed every boundary point, choose a homeomorphism from $T$ to $D$ taking its three edges to three consecutive closed arcs of $\partial D$ with empty triple intersection. The inverse images under $f$ of those arcs would be closed, would cover $D$, and would contain the corresponding boundary arcs. Transporting them to $T$ would contradict the result just proved. Therefore

$$
\boxed{\text{there is no retraction }D\to\partial D}.
$$

For the final statement, use compactness of the three closed arcs inside the corresponding open sets. A finite open cover of a compact metric space admits a closed shrinking, and the shrinking can be chosen to preserve specified compact subsets already lying in the respective open sets. Thus there are closed sets

$$
A\subset P,\qquad B\subset Q,\qquad C\subset R
$$

which cover $D$ and contain $\alpha,\beta,\gamma$, respectively. The disc version of the three-set covering lemma, obtained from the triangle by a homeomorphism taking its edges to the three arcs, gives a point in $A\cap B\cap C$. Since these sets lie in the original open sets,

$$
\boxed{P\cap Q\cap R\ne\varnothing}.
$$

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
