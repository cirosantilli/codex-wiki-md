<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The one-dimensional [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) states: a continuous adapted process $L$, with $L_0=0$, is standard [Brownian motion](../../../../../../brownian-motion-split.md) relative to its filtration if and only if it is a [local martingale](../../../../../../local-martingale.md) and $[L]_t=t$ for all $t$ almost surely.

For necessity, the centered independent Gaussian increments of Brownian motion give both the martingale property and the martingale $L_t^2-t$. The uniqueness characterization of [quadratic variation](../../../../../../quadratic-variation.md) then gives $[L]_t=t$.

For sufficiency fix $\theta\in\mathbb R$. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
E_t=\exp(i\theta L_t+\tfrac12\theta^2t),\qquad dE_t=i\theta E_t\,dL_t.
$$

The second-order term cancels the time derivative because $d[L]_t=dt$. Thus $E$ is a complex local martingale. Its modulus is the deterministic quantity $e^{\theta^2t/2}$, bounded on every finite horizon, so its real and imaginary parts are true martingales by the [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md). For $s<t$,

$$
\mathbb E[e^{i\theta(L_t-L_s)}\mid\mathcal F_s]=e^{-\theta^2(t-s)/2}.
$$

Uniqueness of [characteristic functions](../../../../../../characteristic-function.md) says that the increment has [normal distribution](../../../../../../normal-distribution.md) $N(0,t-s)$ independently of $\mathcal F_s$. Indeed multiplying the identity by any bounded $\mathcal F_s$-measurable variable gives the product characteristic-function identity expressing independence. Iterating over deterministic times gives independent increments. Together with continuity and $L_0=0$, these are precisely the defining properties of standard Brownian motion. If the starting value is a fixed $x$, the same argument identifies $L-x$ as standard Brownian motion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
