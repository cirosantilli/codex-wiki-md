<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

View the oriented square lattice as $(x,n)$ with $x+n$ even, and arrows $(x,n)\to(x\pm1,n+1)$. Each [graph vertex](../../../../../../vertex-graph-theory.md) has two incoming bonds. Start with independent [oriented bond percolation](../../../../../../oriented-bond-percolation.md) of parameter $p$, and declare a site open when at least one of its incoming bonds is open. Its [probability](../../../../../../probability.md) of being open is

$$
r=1-(1-p)^2.
$$

Incoming bond sets for different heads are disjoint, so these site indicators are independent: they are precisely an [oriented site percolation](../../../../../../oriented-site-percolation.md) configuration with parameter $r$.

Every [graph vertex](../../../../../../vertex-graph-theory.md) after the first on an open oriented bond path is open as a site, because its incoming path bond is open. The root's two incoming bonds belong to earlier time layers and are independent of all bonds used by a forward path from the root. Thus the event that the root site is open, of [probability](../../../../../../probability.md) $r$, is independent of bond survival from that root. On their intersection the entire infinite bond path is also an infinite open site path. Hence, writing $\theta_b,\theta_s$ for the two survival [probabilities](../../../../../../probability.md),

$$
\theta_s(1-(1-p)^2)\ge\bigl(1-(1-p)^2\bigr)\theta_b(p).
$$

This is the [incoming-edge coupling of site and bond percolation](../../../../../../incoming-edge-coupling-of-site-and-bond-percolation.md). If site survival is defined conditional on an open root, the extra factor is omitted; the critical [probability](../../../../../../probability.md) is the same. If the model is drawn only in a time half-plane, one can independently sample the root's incoming bonds as auxiliary variables.

For every $p>p_c(\mathrm{bond})$, bond survival is positive by monotonicity and the definition of the critical [probability](../../../../../../probability.md). Therefore $p_c(\mathrm{site})\le1-(1-p)^2$. Let $p$ decrease to the bond critical [probability](../../../../../../probability.md) and use continuity of this polynomial, obtaining

$$
\boxed{p_c(\mathrm{site})\le1-(1-p_c(\mathrm{bond}))^2.}
$$

If the bond critical [probability](../../../../../../probability.md) equals one, the inequality is trivial; no assertion about survival exactly at criticality is used.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
