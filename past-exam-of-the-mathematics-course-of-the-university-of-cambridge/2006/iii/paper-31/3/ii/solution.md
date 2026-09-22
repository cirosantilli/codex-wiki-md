<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\mathcal F_n=\sigma(B_{k2^{-n}}:0\leq k\leq2^n)$. These sigma-fields increase, and their union generates the continuous Brownian path. Let $\mathbf B^{(n)}=S_2(B^{(n)})$ be the polygonal enhancement. Its coordinates are determined by its displacement $b^{(n)}_{s,t}$ and antisymmetric area $a^{(n)}_{s,t}$; the symmetric second level is $\tfrac12 b^{(n)}_{s,t}\otimes b^{(n)}_{s,t}$.

The given conditional-expectation identities imply

$$
b^{(n)}_{s,t}=\mathbb E[B_{s,t}\mid\mathcal F_n],\qquad a^{(n)}_{s,t}=\mathbb E[A_{s,t}\mid\mathcal F_n].
$$

For the second assertion it is important to use area coordinates rather than asserting that the whole tensor signature is a conditional expectation. Write $I_t=\int_0^t\beta\,d\widetilde\beta$. The local off-diagonal second integral is

$$
\mathbb B^{12}_{s,t}=I_t-I_s-\beta_s(\widetilde\beta_t-\widetilde\beta_s).
$$

Conditional on their separate dyadic values, the two independent Brownian components remain independent. Thus the conditional expectation of the product in the last term is $\beta^{(n)}_s(\widetilde\beta^{(n)}_t-\widetilde\beta^{(n)}_s)$. The assumed identity for $I$ gives the polygonal $12$ entry. The reverse entry follows by [integration by parts](../../../../../../integration-by-parts.md), since the product of the two component increments also has the product of their conditional means. Taking the antisymmetric part proves the area identity. Diagonal second levels are recovered from the geometric identity, rather than from a conditional-expectation claim about squares.

For each fixed dyadic time $t$, the first-level and area conditional expectations are uniformly integrable [martingales](../../../../../../martingale-split.md) in $n$. Their targets are measurable with respect to $\mathcal F_\infty=\sigma(\bigcup_n\mathcal F_n)$: Brownian area is a limit of stochastic integral sums determined by the path. The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) gives convergence to $B_t$ and $A_{0,t}$, respectively. The continuous group coordinate formulas then give

$$
\mathbf B^{(n)}_t\longrightarrow\mathbf B_t
$$

at all dyadic times on a common event of probability one.

For the uniform Hölder estimate, fix $\alpha<1/2$ and put $K=\|\mathbf B\|_{\alpha\text{-Hölder};[0,1]}$. The given all-order integrability and the group norm comparison imply

$$
|B_{s,t}|\leq CK|t-s|^\alpha,\qquad |A_{s,t}|\leq C^2K^2|t-s|^{2\alpha}.
$$

Use the conditional-expectation formulas, the conditional [Jensen inequality](../../../../../../jensen-s-inequality.md), and $\mathbb E[K\mid\mathcal F_n]\leq\sqrt{\mathbb E[K^2\mid\mathcal F_n]}$. The group norm comparison yields

$$
d_{CC}(\mathbf B^{(n)}_s,\mathbf B^{(n)}_t)\leq C'\sqrt{\mathbb E[K^2\mid\mathcal F_n]}\,|t-s|^\alpha.
$$

First take all dyadic pairs, a countable collection, and then extend the inequality to all $s,t$ by continuity. Hence the [Brownian rough path martingale Hölder bound](../../../../../../brownian-rough-path-martingale-holder-bound.md) is

$$
\|\mathbf B^{(n)}\|_{\alpha\text{-Hölder}}\leq C'\sqrt{M_n},\qquad M_n=\mathbb E[K^2\mid\mathcal F_n].
$$

For any $q>1$, the [Doob Lp maximal inequality](../../../../../../doob-lp-maximal-inequality.md) gives

$$
\mathbb E\left[\left(\sup_nM_n\right)^q\right]\leq\left(\frac q{q-1}\right)^q\mathbb E[K^{2q}]<\infty.
$$

Therefore

$$
\boxed{\sup_n\|\mathbf B^{(n)}\|_{\alpha\text{-Hölder}}<\infty\quad\text{almost surely}.}
$$

To upgrade convergence from dyadic times to every time simultaneously, apply this bound at one positive exponent $\beta<1/2$. The polygonal enhancements are then equicontinuous in the group metric, with a common finite random constant. For a finite dyadic time net, convergence holds at every net point. The triangle inequality bounds the errors at the remaining times by the two Hölder errors to the nearest net point and the error at that point. First let $n\to\infty$, and then let the net mesh tend to zero. This proves **uniform convergence, and in particular convergence for every $t\in[0,1]$ on one event of probability one**.

There is also convergence in each weaker Hölder [rough path metric](../../../../../../rough-path-metric.md). Uniform convergence of the group coordinates gives uniform convergence of their levelwise increments through the Chen formulas. If $\alpha<\beta<1/2$, the uniform $\beta$ bounds bound the level-$k$ increment differences by a random constant times $|t-s|^{k\beta}$, while their unweighted suprema tend to zero. Interpolating these two bounds proves convergence with denominators $|t-s|^{k\alpha}$, for $k=1,2$. This establishes the [nested polygonal approximation of Brownian rough paths](../../../../../../nested-polygonal-approximation-of-brownian-rough-paths.md) in the topology needed for the support argument.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
