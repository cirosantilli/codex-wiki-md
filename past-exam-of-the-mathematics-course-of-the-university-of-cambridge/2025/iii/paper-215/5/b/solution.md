<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There are $\asymp n^3$ edges. The $n^2$ horizontal cutsets between successive rows perpendicular to the long direction are disjoint and each contains $\asymp n$ unit-conductance edges. [Nash-Williams inequality](../../../../../../nash-williams-inequality.md) gives

$$
R_{\mathrm{eff}}((0,0),(n,n^2))\gtrsim n^2/n=n.
$$

Conversely, spread a unit flow nearly uniformly across the width $n$ while moving it through the $n^2$ long-direction layers, with bounded extra energy to fan out from and collect at the two corner vertices. Its energy is $O(n^2/n)+O(\log n)=O(n)$, so Thomson's principle gives the matching upper bound $R_{\mathrm{eff}}\asymp n$.

The graph is invariant under a half-turn exchanging the two corners, so the two directional hitting-time expectations are equal. The [commute time identity](../../../../../../commute-time-identity.md) therefore yields

$$
\boxed{\mathbb E_{(0,0)}T_{(n,n^2)}
\asymp |E|R_{\mathrm{eff}}\asymp n^3n=n^4.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
