<h1 id="open-mapping-theorem-for-frechet-spaces">Open mapping theorem for Fréchet spaces</h1>

↑ **Parent:** [Open mapping theorem (functional analysis)](open-mapping-theorem-functional-analysis.md)

A continuous surjective [linear map](linear-map.md) between [Fréchet spaces](frechet-space.md) is an [open map](open-map.md). The [Baire category theorem](baire-category-theorem.md) first shows that the closure of the image of every convex balanced zero-neighbourhood is a zero-neighbourhood: the target is the countable union of scalar multiples of this image, and an interior point of its closure can be translated to zero using convexity and symmetry.

To remove the closure, fix a domain zero-neighbourhood $U$ and choose convex balanced zero-neighbourhoods $U_n$ so that every series $\sum_nu_n$, $u_n\in U_n$, converges to a point of $U$. With an increasing defining sequence of [seminorms](seminorm.md) $p_j$, one can ensure $p_j(u_n)<2^{-n}$ for $j\le n$ and make the finitely many [seminorms](seminorm.md) defining $U$ summable within its bounds. Completeness gives convergence. Choose target zero-neighbourhoods $V_n\subset\overline{A(U_n)}$ shrinking to zero. For $y\in V_1$, choose $u_n\in U_n$ successively so that $y-A\sum_{j\le n}u_j\in V_{n+1}$. Density permits each correction. Continuity then gives $y=A\sum_nu_n\in A(U)$, proving openness.

## ↑ Ancestors (6)

1. [Open mapping theorem (functional analysis)](open-mapping-theorem-functional-analysis.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Closed graph theorem for Fréchet spaces](closed-graph-theorem-for-frechet-spaces.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-5/1/solution.md)
