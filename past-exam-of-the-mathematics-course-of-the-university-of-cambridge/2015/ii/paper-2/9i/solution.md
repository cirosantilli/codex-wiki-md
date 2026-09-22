<h1 id="9i/solution">Solution</h1>

↑ **Parent:** [9I](../9i.md)

[Sperner's lemma](../../../../../sperner-s-lemma.md) says that a triangulated triangle whose vertices are labelled $1,2,3$, with each outer vertex having its own label and each boundary edge using only its endpoint labels, contains a small triangle with all three labels. In fact the number of such triangles is odd. Count incidences of small triangles with edges labelled $1,2$. Interior edges contribute twice. On the outer $1,2$ edge, the number of changes between these labels is odd; the other two outer edges contribute zero. A small triangle contributes one incidence if it has all three labels, two if it uses both $1,2$ but not $3$, and zero otherwise. The total parity proves the assertion.

The resulting [no-retraction theorem](../../../../../no-retraction-theorem.md) is: **there is no continuous [retraction](../../../../../retraction.md) of a closed disc onto its boundary**. Work first with a closed triangle $P$. If $r:P\to\partial P$ fixes the boundary, colour each vertex of increasingly fine triangulations by an index of a largest barycentric coordinate of $r(v)$. The largest coordinate is at least $1/3$; on the boundary the colouring satisfies [Sperner's lemma](../../../../../sperner-s-lemma.md). Choose a tricoloured small triangle in each triangulation. By [compactness](../../../../../compact-space.md) and shrinking mesh, a subsequence of their three vertices converges to one point $x$. Continuity forces all three barycentric coordinates of $r(x)$ to be at least $1/3$, so $r(x)$ is the triangle's centre, contradicting $r(x)\in\partial P$. A [homeomorphism](../../../../../homeomorphism.md) of a disc with $P$ proves the disc assertion.

[Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) states that every continuous self-map $F$ of a closed disc has a fixed point. If it had none, the ray from $F(x)$ through $x$ would meet the boundary beyond $x$, continuously in $x$. That intersection defines a [retraction](../../../../../retraction.md), since a boundary point is already the outgoing intersection. This contradicts the [no-retraction theorem](../../../../../no-retraction-theorem.md).

Finally fix $y\in\mathbb R^2$ and define $F_y(x)=y+x-g(x)$. The displacement bound implies $\|F_y(x)-y\|\leq K$, so $F_y$ maps the closed radius-$K$ disc centred at $y$ into itself. [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) gives $F_y(x)=x$, which is exactly $g(x)=y$. Since $y$ was arbitrary, **$g$ is surjective**.

## ↑ Ancestors (10)

1. [9I](../9i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
