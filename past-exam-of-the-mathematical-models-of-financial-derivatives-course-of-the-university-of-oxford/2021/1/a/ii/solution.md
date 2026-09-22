<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $V\in C^{1,2}$, [Itô's formula](../../../../../ito-s-lemma.md) gives

$$
dV=\left(V_t+\mu sV_s+\frac{\sigma^2}{2}V_{ss}\right)dt+\sigma V_s\,dW.
$$

Match the Brownian coefficient with the [self-financing portfolio](../../../../../self-financing-portfolio.md) by choosing the [option delta](../../../../../option-delta.md) $\phi=V_s$ and bond value $\psi B=V-sV_s$. Equating drifts cancels the physical drift $\mu$ and gives

$$
\boxed{V_t+rsV_s+\frac{\sigma^2}{2}V_{ss}-rV=0,
\quad (t,s)\in[0,T)\times\mathbb R,\qquad V(T,s)=F(s).}
$$

This is the [pricing equation for a linear asset with additive noise](../../../../../pricing-equation-for-a-linear-asset-with-additive-noise.md). Its spatial [domain](../../../../../domain-mathematical-analysis.md) is the whole [real line](../../../../../real-line.md), because the asset can be negative. In particular the diffusion term is $\sigma^2V_{ss}/2$, not $\sigma^2s^2V_{ss}/2$. The derivation is [delta hedging](../../../../../delta-hedge.md) and does not impose a boundary condition at $s=0$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../../split.md)
6. [Mathematical models of financial derivatives course of the University of Oxford](../../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
