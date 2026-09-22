<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $V(t,r)$ sufficiently smooth, [Itô formula](../../../../../../ito-s-lemma.md) under the physical measure gives

$$
dV=\left(V_t+bV_r+\frac12\sigma^2V_{rr}\right)dt+\sigma V_r\,dW.
$$

Hence $m=V_t+bV_r+\sigma^2V_{rr}/2$ and $s=\sigma V_r$. Substitute these into the common risk-price condition $m-rV=\theta s$ from part (b), obtaining the [Cox-Ross short-rate pricing equation](../../../../../../cox-ross-short-rate-pricing-equation.md)

$$
\boxed{V_t+(b-\sigma\theta)V_r+\frac12\sigma^2V_{rr}-rV=0.}
$$

For a terminal payoff $H(r_T)$ the final condition is $V(T,r)=H(r)$. Writing prices as functions of $(t,r)$ requires the relevant [Markov](../../../../../../markov-property.md) state to be sufficient for the claim; a path-dependent payoff generally requires additional state variables. The negative sign in $b-\sigma\theta$ is the adjustment from physical to risk-neutral rate drift.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
