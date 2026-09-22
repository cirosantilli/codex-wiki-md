<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The region $A_h$ usually has a curved boundary, so sampling uniformly inside it directly is inconvenient. [Rejection sampling](../../../../../../rejection-sampling.md) replaces it by an easily sampled envelope, usually a rectangle. Choose finite bounds $a,b_-,b_+$ with

$$
a\ge\sup_x\sqrt{h(x)},\qquad b_-\le\min(0,\inf_x x\sqrt{h(x)}),\qquad b_+\ge\max(0,\sup_x x\sqrt{h(x)}).
$$

Then $A_h\subseteq(0,a)\times(b_-,b_+)$ up to null boundaries. A general rectangle algorithm uses only [independent](../../../../../../independent-random-variables.md) uniform deviates: draw $U_1,U_2$ on $(0,1)$, set $u=aU_1$, $v=b_-+(b_+-b_-)U_2$, and return $v/u$ if $u^2\le h(v/u)$; otherwise repeat. If a numerical generator returns $u=0$, discard that draw before division. No knowledge of $Z$ is required to run the method. Its acceptance rate is the ratio of the two areas:

$$
\boxed{r=\frac{\operatorname{area}(A_h)}{\operatorname{area}(B)}=\frac{Z}{2a(b_+-b_-)}.}
$$

More generally the same area ratio applies to any finite-area envelope $B$ sampled uniformly. A change in the proportionality constant of $h$ scales both ratio coordinates and their areas consistently.

Finite rectangle bounds are a real condition, not a consequence of integrability alone. For instance $h(x)=(1+|x|)^{-3/2}$ is integrable, but $|x|\sqrt{h(x)}$ is unbounded. A [finite-area envelope for a ratio-of-uniforms region](../../../../../../finite-area-envelope-for-a-ratio-of-uniforms-region.md) gives a general extension: choose a finite-area open envelope containing $A_h$, decompose it up to null boundaries into countably many disjoint rectangles, and select a rectangle with probability proportional to its area using a uniform draw and cumulative probabilities. Use two more uniforms to sample within it, then apply the same acceptance test. This samples the envelope uniformly and has acceptance $Z/(2\operatorname{area}(B))$. Such envelopes exist for every finite-area measurable $A_h$; obtaining usable bounds or an effective rectangle decomposition is density-specific. The finite-rectangle version above is the usual practical implementation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
