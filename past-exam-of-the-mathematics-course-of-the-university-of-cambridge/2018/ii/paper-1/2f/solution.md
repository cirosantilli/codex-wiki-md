<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

[Sperner's lemma](../../../../../sperner-s-lemma.md) says that if a [triangle](../../../../../triangle.md) is triangulated, its vertices are labelled $1,2,3$, and label $i$ is forbidden on the edge opposite vertex $i$, then an odd number of small triangles have all three labels.

To prove it, count incidences with edges whose endpoint labels are $1$ and $2$. Along the outer $12$-edge, the labels begin at $1$ and end at $2$, so the number of $12$ transitions is odd; no other boundary edge contributes. An interior edge contributes twice. A small triangle contributes an odd number precisely when its three labels are $1,2,3$: a triangle using only $1,2$ contributes two, and every other non-tricoloured triangle contributes zero. The number of tricoloured triangles is therefore odd.

Now suppose the closed sets $A_i$ in the question existed. Let $d_i(x)$ be the [distance from a point to a closed set](../../../../../distance-from-a-point-to-a-closed-set.md) $A_i$. Empty triple intersection makes $d_1+d_2+d_3>0$, so

$$
r(x)=\frac{d_1(x)v_1+d_2(x)v_2+d_3(x)v_3}
{d_1(x)+d_2(x)+d_3(x)}
$$

is a [continuous function](../../../../../continuous-function.md) from the large triangle to itself, where $v_i$ is the vertex opposite $\alpha_i$. Since the $A_i$ cover the triangle, at least one $d_i(x)$ vanishes, so $r(x)$ always lies on the boundary. On $\alpha_i\subseteq A_i$, its $i$th barycentric coordinate vanishes, hence $r(\alpha_i)\subseteq\alpha_i$. Thus $r$ is face-preserving on the boundary; its boundary restriction is homotopic there to the identity by the straight-line homotopy. This would give a map from the triangle into its boundary whose boundary degree is one, contradicting the [no-retraction theorem](../../../../../no-retraction-theorem.md), the standard topological consequence of Sperner's lemma. **Therefore the three closed sets must have a common point.**

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
