<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $t(u)$ be the inverse image-capacity clock. Part (a) and the [quadratic variation of a stochastic integral](../../../../../../quadratic-variation-of-a-stochastic-integral.md) give

$$
\widetilde\xi_u=\xi^*_{t(u)},\qquad [\widetilde\xi]_u=6u.
$$

The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md), or the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md), now shows that $\widetilde\xi_u/\sqrt6$ is standard [Brownian motion](../../../../../../brownian-motion-split.md) up to the terminal image time. If that terminal clock is finite, it can be extended by a fresh Brownian continuation; this does not assert anything about the subsequent image trace. The initial value is zero because $\Phi(0)=0$.

Differentiating the image [Loewner chain](../../../../../../loewner-chain.md) with respect to its own [half-plane capacity](../../../../../../half-plane-capacity.md) time gives

$$
\partial_u\widetilde g_u(z)=\frac2{\widetilde g_u(z)-\widetilde\xi_u},\qquad
\widetilde g_u=g^*_{t(u)}.
$$

Thus, until its first hit of $[1,\infty)$, the reparametrized image $\Phi(\gamma)$ has the ordinary chordal [SLE](../../../../../../schramm-loewner-evolution.md) law from $0$ to infinity. This follows from the uniqueness of the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) for a given continuous driver; the continuous [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) is recovered from the inverse-map limit. Localization can be removed by exhausting times strictly before this [boundary](../../../../../../boundary-of-a-set.md) contact. The terminal event is defined from the trace itself, so equality of the stopped trace laws follows as well.

On the other hand, the definition of [Conformal invariance of SLE](../../../../../../conformal-invariance-of-sle.md) says that the full unparameterized image $\Phi(\gamma)$ has the law of chordal $\operatorname{SLE}_6$ from $\Phi(0)=0$ to $\Phi(\infty)=1$, namely the law of $\gamma'$. Its stopping event at $[1,\infty)$ is exactly the image of the original stopping event at $(-\infty,-1]$. Therefore the same stopped image has both laws: ordinary $\operatorname{SLE}_6$ from $0$ to infinity stopped at $T$, and $\operatorname{SLE}_6$ from $0$ to $1$ stopped at $T'$. We conclude

$$
\boxed{(\gamma_t:0\leq t<T)\ \overset d=\ (\gamma'_t:0\leq t<T')
\quad\text{as curves up to increasing reparametrization}.}
$$

The statement does not identify $T$ with $T'$ in their original clocks. It is [target-change locality of SLE6](../../../../../../target-change-locality-of-sle6.md), derived from the zero drift and capacity time change rather than assumed as a theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
