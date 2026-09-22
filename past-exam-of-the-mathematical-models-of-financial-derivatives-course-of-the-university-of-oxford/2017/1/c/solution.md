<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The differential operator in part [b](../b.md) is the [infinitesimal generator](../../../../infinitesimal-generator-stochastic-processes.md) of the auxiliary [diffusion process](../../../../markov-diffusion.md) $dS_u=rS_u\,du+\sigma\,dW_u$, with killing rate $r$. The [Feynman-Kac formula](../../../../feynman-kac-formula.md) therefore gives

$$
\boxed{V(S,t)=e^{-r(T-t)}\mathbb E^{\mathbb Q}[P_{\mathrm o}(S_T)\mid S_t=S].}
$$

Equivalently, [Itô's formula](../../../../ito-s-lemma.md) makes $e^{-r(u-t)}V(S_u,u)$ a [local martingale](../../../../local-martingale.md) under these dynamics; under appropriate growth and integrability assumptions it is a [martingale](../../../../martingale-split.md), whose terminal [conditional expectation](../../../../conditional-expectation.md) yields the same formula. The expectation uses the drift-$r$ law, rather than the physical drift-$\alpha$ law in part [a](../a.md). This is [risk-neutral pricing](../../../../risk-neutral-pricing.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
