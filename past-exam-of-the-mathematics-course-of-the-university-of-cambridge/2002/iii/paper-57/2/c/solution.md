<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Not in general. A [food web](../../../../../../food-web.md) with [Lotka-Volterra equations](../../../../../../lotka-volterra-equations.md) has per-capita balances $\dot X_i/X_i=r_i+\sum_jA_{ij}X_j$. If all species remain bounded above and away from zero, averaging requires $r+A\overline X=0$ with positive [means](../../../../../../expected-value.md). Many webs have no feasible positive solution. Even a feasible solution does not ensure stability or persistence when the weighted [skew-symmetric matrix](../../../../../../skew-symmetric-matrix.md) structure and its coercive [first integral](../../../../../../first-integral.md) are absent.

A simple resource shared by two consumers already illustrates [competitive exclusion principle](../../../../../../competitive-exclusion-principle.md). Suppose their per-capita equations are $\dot Y/Y=cX-d$ and $\dot Z/Z=eX-f$. Then

$$
\frac d{dt}\left(\frac{\log Y}{c}-\frac{\log Z}{e}\right)=-\frac dc+\frac fe.
$$

If $d/c\ne f/e$, the ratio has exponential drift, incompatible with bounded persistence of both consumers. The lower break-even-resource consumer has the advantage; equal break-even requirements are a special neutral balance, not generic coexistence. More complicated feeding links can provide additional niches, but positive coefficients and a larger web do not by themselves guarantee that every species survives. One must test feasibility, invasion into the relevant boundary states and stability, with explicit assumptions about resource renewal and self-limitation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
