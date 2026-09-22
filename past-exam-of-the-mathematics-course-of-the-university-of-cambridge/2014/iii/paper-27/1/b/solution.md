<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $V=\langle X\rangle$. Applying the [Itô formula](../../../../../../ito-s-lemma.md) and the [Itô product rule](../../../../../../ito-product-rule.md) gives

$$
d(X^4)=4X^3\,dX+6X^2\,dV,\qquad d(X^2V)=2XV\,dX+(V+X^2)\,dV,\qquad d(V^2)=2V\,dV.
$$

The finite-variation terms cancel in the prescribed combination, leaving

$$
dY_t=(4X_t^3-12X_tV_t)\,dX_t.
$$

Thus $Y$ is initially a [continuous local martingale](../../../../../../continuous-local-martingale.md). It is a true [martingale](../../../../../../martingale-split.md), not merely local. On each fixed horizon $T$,

$$
\sup_{s\leq T}|Y_s|\leq S_T^4+6S_T^2V_T+3V_T^2.
$$

Part (a) with $p=4$, the assumed bracket moments and [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) make this bound integrable. The [integrable-supremum martingale criterion](../../../../../../integrable-supremum-martingale-criterion.md) now applies, by localization and dominated conditional expectations. The same reasoning makes $X^2-V$ a [martingale](../../../../../../martingale-split.md), so $\mathbb EV_t=\mathbb EX_t^2=t$.

The zero [covariance](../../../../../../covariance.md) now means $\mathbb E(X_t^2V_t)=t^2$. Since $Y_0=0$ and $\mathbb EY_t=0$,

$$
\boxed{\mathbb EX_t^4=6t^2-3\mathbb EV_t^2=3t^2-3\operatorname{Var}(V_t)\leq3t^2.}
$$

This is the [fourth-moment deficit and bracket variance identity](../../../../../../fourth-moment-deficit-and-bracket-variance-identity.md). If equality holds for every $t$, then $V_t=t$ almost surely for each $t$. Take a single probability-one event for all rational times and use continuity to obtain $V_t=t$ simultaneously for all times. The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) then proves **$X$ is [Brownian motion](../../../../../../brownian-motion-split.md) in its given filtration**. A proof of that characterization by conditional characteristic functions is included in Question 2(a).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
