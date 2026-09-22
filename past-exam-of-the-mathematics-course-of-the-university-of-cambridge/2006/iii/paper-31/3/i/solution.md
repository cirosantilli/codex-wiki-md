<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [Brownian motion](../../../../../../brownian-motion-split.md) $B$ starting at zero, define its [enhanced Brownian motion](../../../../../../enhanced-brownian-motion.md) by the Stratonovich second level:

$$
\mathbf B_{s,t}=\left(1,B_t-B_s,\mathbb B_{s,t}\right),\qquad \mathbb B_{s,t}^{ij}=\int_s^t(B_r^i-B_s^i)\circ dB_r^j.
$$

The associated group-valued path is $\mathbf B_t=\mathbf B_{0,t}$. The [Stratonovich chain rule](../../../../../../stratonovich-chain-rule.md) gives

$$
\mathbb B_{s,t}^{ij}+\mathbb B_{s,t}^{ji}=B_{s,t}^iB_{s,t}^j.
$$

Consequently its symmetric second level is $\tfrac12 B_{s,t}\otimes B_{s,t}$ and the remaining antisymmetric part $A_{s,t}=\tfrac12(\mathbb B_{s,t}-\mathbb B_{s,t}^{\mathsf T})$ is [Lévy area](../../../../../../levy-area.md). Splitting the integral at $u$ proves the [Chen identity](../../../../../../chen-identity.md), so these increments lie in $G^2(\mathbb R^d)$ and are the relative increments of $\mathbf B_t$.

The group norm for the [Carnot-Carathéodory distance](../../../../../../carnot-caratheodory-distance.md) is comparable to $|B_{s,t}|+|A_{s,t}|^{1/2}$. The planar construction in Question 2 extends to dimension $d$: prescribe every coordinate-plane area with a closed rectangle, concatenate these central-area loops, and finish with the displacement segment. The converse bound follows from length bounds on displacement and on each area integral. Thus the comparison constants depend only on $d$.

Brownian scaling and stationarity of increments imply that $(B_{s,t},A_{s,t})$ has the distribution of $(\sqrt{t-s}\,B_{0,1},(t-s)A_{0,1})$. The permitted moment estimates for Lévy area, together with Gaussian moments of Brownian displacement, therefore give, for every finite $q\geq1$,

$$
\mathbb E\bigl[d_{CC}(\mathbf B_s,\mathbf B_t)^q\bigr]\leq C_q|t-s|^{q/2}.
$$

This also verifies the hypothesis of the metric-valued [Kolmogorov continuity theorem](../../../../../../kolmogorov-continuity-theorem.md). We give the dyadic argument to obtain a simultaneous version explicitly.

Fix $0<\beta<1/2$ and choose $q$ so large that $q(1/2-\beta)>1$. The [Markov inequality](../../../../../../markov-inequality.md) and a union bound give

$$
\mathbb P\left(\max_{0\leq k<2^n}d_{CC}(\mathbf B_{k2^{-n}},\mathbf B_{(k+1)2^{-n}})>2^{-n\beta}\right)\leq C_q2^{-n(q(1/2-\beta)-1)}.
$$

The right-hand side is summable. By the [Borel-Cantelli first lemma](../../../../../../borel-cantelli-first-lemma.md), almost surely there is a finite random constant $K_\beta$ bounding every adjacent dyadic increment by $K_\beta2^{-n\beta}$, including the finitely many exceptional levels.

Decompose any interval with dyadic endpoints into successive dyadic intervals, with at most two intervals of each size and no size exceeding its length. The metric triangle inequality and the sum of the geometric series give

$$
d_{CC}(\mathbf B_s,\mathbf B_t)\leq C_\beta K_\beta|t-s|^\beta
$$

for all dyadic $s,t$. The finite-dimensional Carnot group is complete, so the path extends uniquely from dyadic times to a continuous $\beta$-Hölder path. At each fixed time the original stochastic enhancement and its values at approaching dyadic times converge in probability by the moment estimate. The extension has the same limit almost surely, hence is a modification of the original enhancement.

Perform this construction on one countable sequence of exponents increasing to $1/2$. The extensions agree on the dense set of dyadic times, so they give one modification that is Hölder at every exponent below $1/2$. On $[0,1]$, a $\beta$-Hölder estimate implies the same estimate at every $0\leq\alpha\leq\beta$. Therefore

$$
\boxed{\|\mathbf B\|_{\alpha\text{-Hölder};[0,1]}<\infty\quad\text{almost surely for every fixed }\alpha<\tfrac12.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
