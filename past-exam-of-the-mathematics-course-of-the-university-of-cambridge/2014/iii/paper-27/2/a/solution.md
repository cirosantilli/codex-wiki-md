<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V_t=\langle M\rangle_t$, and first suppose $V_\infty=\infty$ almost surely in addition to strict increase. The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) says that

$$
T_u=\inf\{t:V_t>u\},\qquad\mathcal G_u=\mathcal F_{T_u},\qquad B_u=M_{T_u}
$$

define a [Brownian motion](../../../../../../brownian-motion-split.md) $B$ in the time-changed filtration and give

$$
\boxed{M_t=B_{V_t}.}
$$

Each $T_u$ is a [stopping time](../../../../../../stopping-time.md) and is finite. Continuity and strict increase of $V$ make $u\mapsto T_u$ continuous, $V_{T_u}=u$ and $T_{V_t}=t$.

Here are the [martingale](../../../../../../martingale-split.md) details behind this [inverse-clock proof of the Dambis-Dubins-Schwarz theorem](../../../../../../inverse-clock-proof-of-the-dambis-dubins-schwarz-theorem.md). Stopping a [continuous local martingale](../../../../../../continuous-local-martingale.md) when its bracket reaches $n$ makes it an [L2-bounded continuous martingale](../../../../../../l2-bounded-continuous-martingale.md). This follows from the stopped [Itô isometry](../../../../../../ito-isometry.md) or from the $p=2$ estimate proved in Question 1(a), applied after localization. In particular it is [uniformly integrable](../../../../../../uniform-integrability.md), and optional sampling is valid even at an unbounded [stopping time](../../../../../../stopping-time.md) by taking limits. Applying this to $M$ stopped at $T_n$ shows that $(M_{T_{u\wedge n}})_{u\geq0}$ is a [martingale](../../../../../../martingale-split.md). Thus $B$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md). Time-changing $M^2-V$ in the same way shows $B_u^2-u$ is a [local martingale](../../../../../../local-martingale.md), so $\langle B\rangle_u=u$.

For completeness, the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) follows directly from the [Itô formula](../../../../../../ito-s-lemma.md). If a [continuous local martingale](../../../../../../continuous-local-martingale.md) $N$, starting at zero, has bracket $u$, then

$$
\exp\left(i\theta N_u+\frac{\theta^2u}{2}\right)
$$

is a complex [local martingale](../../../../../../local-martingale.md). Its modulus is bounded on each deterministic finite horizon, so it is a true [martingale](../../../../../../martingale-split.md) there. Consequently

$$
\mathbb E\left[e^{i\theta(N_u-N_v)}\mid\mathcal G_v\right]=e^{-\theta^2(u-v)/2}\qquad(v\leq u).
$$

Conditional characteristic functions give Gaussian increments independent of the past. Iterating this identity gives independent increments, and continuity completes the Brownian characterization. The identical vector argument proves the [Lévy characterization of multidimensional Brownian motion](../../../../../../levy-characterization-of-multidimensional-brownian-motion.md) when the bracket matrix is $uI$.

The printed strict-increase hypothesis does not imply $V_\infty=\infty$. For example, $M_t=\int_0^te^{-s}\,dW_s$ has strictly increasing bracket $(1-e^{-2t})/2$. To state the theorem under exactly the printed hypothesis, allow an independent enlargement of the probability space if the terminal clock $L=V_\infty$ can be finite.

On $\{L<\infty\}$ the [martingale](../../../../../../martingale-split.md) $M$ has a finite terminal limit. Indeed, stopping at each bracket level $n$ gives an [L2-bounded continuous martingale](../../../../../../l2-bounded-continuous-martingale.md) which converges; on $\{V_\infty<n\}$ the stopped process is the original one. This proves the [finite-bracket convergence lemma](../../../../../../finite-bracket-convergence-lemma.md). Set $T_u=\infty$ when $u\geq L$ and continue $N_u=M_{T_u}$ by that terminal limit. The optional-sampling argument just given makes $N$ a [continuous local martingale](../../../../../../continuous-local-martingale.md) with bracket $u\wedge L$. Moreover $L$ is a [stopping time](../../../../../../stopping-time.md) in $\mathcal G_u=\mathcal F_{T_u}$.

On a product extension add an independent [Brownian motion](../../../../../../brownian-motion-split.md) $\beta$ in clock time, and put

$$
\widetilde B_u=N_u+\int_0^u\mathbf1_{\{s>L\}}\,d\beta_s.
$$

The two summands have zero [quadratic covariation](../../../../../../quadratic-covariation.md), and their brackets are $u\wedge L$ and $(u-L)^+$. Thus $\langle\widetilde B\rangle_u=u$; the proved characterization makes $\widetilde B$ Brownian. Since $V_t<L$ at every finite $t$ when $L$ is finite, $M_t=\widetilde B_{V_t}$ still holds. This is the [finite-lifetime extension of the Dambis-Dubins-Schwarz theorem](../../../../../../finite-lifetime-extension-of-the-dambis-dubins-schwarz-theorem.md). **An infinite clock gives [Brownian motion](../../../../../../brownian-motion-split.md) on the original space; a finite clock may require the independent extension.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
