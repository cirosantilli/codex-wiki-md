<h1 id="5/with-transaction-costs/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For [marginal utility pricing with proportional transaction costs](../../../../../../../marginal-utility-pricing-with-proportional-transaction-costs.md), if $X-\varepsilon\geq0$ almost surely or $-X-\varepsilon\geq0$ almost surely, the source's second alternative holds. Otherwise $\mathbb P(X<\varepsilon)>0$ and $\mathbb P(X>-\varepsilon)>0$. The [Fatou lemma](../../../../../../../fatou-s-lemma.md) argument now gives $G(\theta)\to-\infty$ at both ends, since a large positive holding loses on the first event and a large negative holding loses on the second. Let $\theta_*$ be a finite maximizer.

If $\theta_*>0$, set $Z_0=U'(\theta_*(X-\varepsilon))$. The derivative condition gives $\mathbb E[XZ_0]=\varepsilon\mathbb E Z_0$. As before, split according to $|X-\varepsilon|\geq1$ to obtain [integrability](../../../../../../../integrability.md) of $Z_0$ from the absolutely integrable derivative, with a compact-set bound on the complement. If $\theta_*<0$, use $Z_0=U'(\theta_*(X+\varepsilon))$ and obtain $\mathbb E[XZ_0]=-\varepsilon\mathbb E Z_0$. In either case normalize $Z=Z_0/\mathbb E Z_0$; then $Z>0$, $\mathbb EZ=1$, and $XZ$ is absolutely integrable.

If $\theta_*=0$, a concave maximum has $G'_-(0)\geq0\geq G'_+(0)$, so $\mathbb EX\in[-\varepsilon,\varepsilon]$. Choose $Z=1$. **In every case of this first alternative, $\boxed{\mathbb E[XZ]\in[-\varepsilon,\varepsilon]}$.** The normalization establishes a stronger, economically meaningful statement than the literal unnormalized condition: the expected gain under the resulting density lies inside the transaction-cost spread.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [With transaction costs](../../with-transaction-costs.md)
3. [5](../../../5.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
