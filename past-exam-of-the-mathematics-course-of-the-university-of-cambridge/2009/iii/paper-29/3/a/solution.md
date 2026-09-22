<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) states that if $N$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md) with $N_0=0$ and $[N]_\infty=\infty$ almost surely, then for $\sigma_r=\inf\{t:[N]_t>r\}$, $W_r=N_{\sigma_r}$ is [Brownian motion](../../../../../../brownian-motion-split.md) in $\mathcal F_{\sigma_r}$ and $N_t=W_{[N]_t}$. If the terminal bracket is finite, [Brownian motion](../../../../../../brownian-motion-split.md) can be continued beyond it on an extension of the probability space. For a nonzero initial value, apply the theorem to $N-N_0$.

Apply time change to the vector $(M^1-M^1_0,M^2-M^2_0)$ with the common bracket $A$. The time-change theorem for [continuous local martingales](../../../../../../continuous-local-martingale.md) says that at inverse bracket times the processes remain [continuous local martingales](../../../../../../continuous-local-martingale.md) in the time-changed filtration and their [quadratic covariations](../../../../../../quadratic-covariation.md) are composed with those times. Since $A$ is continuous and unbounded, $A_{\sigma_r}=r$, giving

$$
[\widetilde B^i,\widetilde B^j]_r=\delta_{ij}r,\qquad\widetilde B_r^i=M^i_{\sigma_r}-M^i_0.
$$

The [Lévy characterization of multidimensional Brownian motion](../../../../../../levy-characterization-of-multidimensional-brownian-motion.md) states that a zero-starting continuous vector [local martingale](../../../../../../local-martingale.md) with bracket matrix $rI$ is standard multidimensional [Brownian motion](../../../../../../brownian-motion-split.md). Thus $\widetilde B$ is standard two-dimensional [Brownian motion](../../../../../../brownian-motion-split.md); this step establishes the joint property, not merely the one-dimensional property of each coordinate.

The printed inverse is $\tau_r=\inf\{t:A_t\geq r\}$. For $r>0$ it is a [stopping time](../../../../../../stopping-time.md), since $\{\tau_r\leq t\}=\{A_t\geq r\}$, and $\tau_0=0$. The [martingale](../../../../../../martingale-split.md) is constant on each flat interval of $A$, as follows from its Dambis-Dubins-Schwarz representation. Hence $M^i_{\tau_r}=M^i_{\sigma_r}$, including any initial flat interval. Moreover $\mathcal F_{\tau_r}\subseteq\mathcal F_{\sigma_r}$. The common Brownian process is adapted to the smaller filtration, and its increments are independent of the larger past, so they are independent of the smaller past as well. Therefore the [common-clock time change of orthogonal local martingales](../../../../../../common-clock-time-change-of-orthogonal-local-martingales.md) gives

$$
\boxed{B_r=(M^1_{\tau_r},M^2_{\tau_r})\text{ is Brownian motion started at }(M^1_0,M^2_0)\text{ in }\mathcal G_r=\mathcal F_{\tau_r}.}
$$

If [Brownian motion](../../../../../../brownian-motion-split.md) is understood to start at zero, the centered vector $B_r-B_0$ is the standard [Brownian motion](../../../../../../brownian-motion-split.md). Retaining the initial vector is the convention required in part (c).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
