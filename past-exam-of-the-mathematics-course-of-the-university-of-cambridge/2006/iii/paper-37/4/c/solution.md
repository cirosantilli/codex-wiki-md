<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The previous part and the permitted assumption $p_c(\mathrm{bond})<1$ imply $p_c(\mathrm{site})<1$. We build an independent [oriented site percolation](../../../../../../oriented-site-percolation.md) process whose open paths carry contact-process infections, and whose site [probability](../../../../../../probability.md) tends to one as $\lambda$ increases.

Use the [graphical representation of the contact process](../../../../../../graphical-representation-of-the-contact-process.md) with recovery rate one and per-neighbour arrow rate $\lambda$. Fix $\delta>0$. On the parity lattice $(x,n)$ with $n\ge0$ and $x+n$ even, declare $(x,n)$ good if there is no recovery mark at $x$ during $[(n-1)\delta,(n+1)\delta]$, and there is at least one arrow from $x$ to each of $x-1,x+1$ during $[n\delta,(n+1)\delta]$. Extend the Poisson clocks to negative times solely to define the root event; the process itself still starts at time zero. Goodness has [probability](../../../../../../probability.md)

$$
q(\lambda,\delta)=e^{-2\delta}(1-e^{-\lambda\delta})^2.
$$

The independence here is important. At a fixed spatial site $x$, the allowed time indices differ by two. Its two-unit recovery intervals therefore have disjoint interiors, and its outgoing-arrow intervals are disjoint. At different spatial sites, recovery clocks are different and outgoing arrows have different tails, hence use different directed-edge clocks. Every defining random input belongs to just one parity site's event, up to deterministic interval endpoints at which a Poisson mark has [probability](../../../../../../probability.md) zero. Thus the good-site indicators really are independent, with common [probability](../../../../../../probability.md) $q$; no theorem about dependent percolation is needed.

Suppose $(x,n)$ and $(x\pm1,n+1)$ are both good and $x$ is infected at time $n\delta$. The source has no recovery before $(n+1)\delta$, and it sends an arrow to the chosen neighbour during that interval. The target's good event excludes recovery throughout $[n\delta,(n+2)\delta]$, so the target is infected at time $(n+1)\delta$. Induction shows that any infinite oriented path of good sites starting at $(0,0)$ sustains infection at every time layer. Along each transmitting interval there is always an infected site, so the [contact process](../../../../../../contact-process.md) never reaches its empty absorbing state.

Take $\delta=\lambda^{-1/2}$. Then

$$
q(\lambda,\lambda^{-1/2})=e^{-2/\sqrt\lambda}(1-e^{-\sqrt\lambda})^2\longrightarrow1.
$$

For some finite $\lambda$ it exceeds $p_c(\mathrm{site})$, and the good-site process has positive survival [probability](../../../../../../probability.md). The [contact process](../../../../../../contact-process.md) begun from the origin therefore also survives with positive [probability](../../../../../../probability.md). Hence

$$
\boxed{\lambda_c<\infty.}
$$

This is the [independent oriented-percolation comparison for the contact process](../../../../../../independent-oriented-percolation-comparison-for-the-contact-process.md). If the infection convention assigns total rate $\lambda$ rather than rate $\lambda$ to each of the two neighbours, replace the arrow rate by $\lambda/2$; the same limit proves the same finiteness conclusion.

## ↑ Ancestors (11)

1. [C](../c.md)
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
