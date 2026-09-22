<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [self-financing portfolio](../../../../self-financing-portfolio.md) with $\Delta_t$ units of the traded asset and the remainder in the [continuous-time bank account](../../../../continuous-time-bank-account.md). If its value equals $V(S_t,t)$, its [self-financing condition](../../../../self-financing-condition.md) is

$$
dV=\Delta_t\,dS_t+r(V-\Delta_tS_t)\,dt.
$$

Meanwhile [Itô's formula](../../../../ito-s-lemma.md) gives

$$
dV=(V_t+\alpha S_tV_S+\tfrac12\sigma^2V_{SS})\,dt+\sigma V_S\,dW_t.
$$

Matching the [Brownian motion](../../../../brownian-motion-split.md) coefficients gives the [delta hedge](../../../../delta-hedge.md) $\Delta_t=V_S$. Matching drifts then cancels the physical drift $\alpha$, leaving the [pricing equation for a linear asset with additive noise](../../../../pricing-equation-for-a-linear-asset-with-additive-noise.md):

$$
\boxed{V_t+\frac12\sigma^2V_{SS}+rSV_S-rV=0,\qquad V(S,T)=P_{\mathrm o}(S).}
$$

The domain is the full [real line](../../../../real-line.md): additive noise can take the asset through zero. The [diffusion coefficient](../../../../diffusion-coefficient.md) is $\sigma$, so the second-derivative term has no factor $S^2$. As usual, the replication argument assumes suitable differentiability and an [admissible trading strategy](../../../../admissible-trading-strategy.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
