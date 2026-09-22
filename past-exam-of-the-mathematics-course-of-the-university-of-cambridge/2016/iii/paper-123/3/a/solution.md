<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Normalize $v_K$ by $v_K(\pi_K)=1$ and put $v_K(0)=+\infty$. Write $f(X)=\sum_{j=0}^d a_jX^j$, with $a_d=1$ and $a_0\ne0$. In the usual coefficient-exponent convention, the [Newton polygon](../../../../../../newton-polygon.md) $N_K(f)$ is the lower boundary of the [convex hull](../../../../../../convex-hull.md) of the upward vertical rays starting at

$$
\boxed{(j,v_K(a_j))\qquad(0\leq j\leq d,\ a_j\ne0).}
$$

It runs from $(0,v_K(a_0))$ to $(d,0)$, with nondecreasing slopes from left to right. Zero coefficients contribute no finite point. Equivalently it is the largest convex piecewise-linear function lying below all these coefficient points.

The [Newton polygon root valuation theorem](../../../../../../newton-polygon-root-valuation-theorem.md) says that a segment of slope $s$ and horizontal length $r$ accounts for exactly $r$ roots of [valuation](../../../../../../valuation.md) $-s$, counted with multiplicity, using the extended [valuation](../../../../../../valuation.md) on an [algebraic closure](../../../../../../algebraic-closure.md). The nonzero constant coefficient excludes a zero root.

For a short justification, use the [weighted Gauss valuation](../../../../../../weighted-gauss-valuation.md) $w_t(P)=\min_j(v(c_j)+jt)$ for $P=\sum c_jX^j$. It is multiplicative: after scaling $X$ by an element of [valuation](../../../../../../valuation.md) $t$ in a valued extension, the initial nonzero residue polynomials multiply without vanishing. Rational $t$ suffice. Factoring a monic [polynomial](../../../../../../polynomial-split.md) into linear factors gives $w_t(f)=\sum_r\min(t,v(r))$. This supporting-line function changes derivative at precisely the root [valuations](../../../../../../valuation.md); its derivative drops count their multiplicities. Supporting lines to the lower polygon have slope $-t$, proving the sign and horizontal-length assertion.

**Slope convention for part (b).** Reflecting the horizontal axis, by plotting $(d-j,v_K(a_j))$, produces the [reflected Newton polygon convention](../../../../../../reflected-newton-polygon-convention.md); its slopes are the root [valuations](../../../../../../valuation.md) themselves. Part (b)'s wording with $m$ instead of $-m$ is correct under this positive-root-[valuation](../../../../../../valuation.md) convention. The proof below gives both forms explicitly, so the result does not depend on silently changing the sign.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
