<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The diffusion associated with the displayed pricing equation is $d\widetilde S_s=0.04\widetilde S_sds+0.2\widetilde S_s dW_s$. For $Y_s=e^{-0.05s}V(s,\widetilde S_s)$, [Itô's formula](../../../../../ito-s-lemma.md) gives

$$
dY_s=e^{-0.05s}\bigl(V_t+0.04\widetilde S_sV_S+0.02\widetilde S_s^2V_{SS}-0.05V\bigr)ds
+e^{-0.05s}0.2\widetilde S_sV_S\,dW_s.
$$

The drift vanishes by the PDE. Under the usual integrability conditions for the payoff and solution, localization and conditional expectation make $Y$ a true martingale; for polynomial-growth data the lognormal moment bounds provide the needed integrability. Applying the terminal condition yields the [Feynman-Kac formula](../../../../../feynman-kac-formula.md)

$$
\boxed{V(t,S)=e^{-0.05(T-t)}\mathbb E[\Psi(\widetilde S_T)\mid\widetilde S_t=S].}
$$

The printed diffusion contains an additional undefined factor $\sigma$ multiplying $0.2\widetilde S_s dW_s$. If literally retained, its second-order generator coefficient would be $0.02\sigma^2S^2$, so the requested representation would correspond to that different PDE unless $\sigma^2=1$. The formula above uses the volatility $0.2$ specified by the stock model and by part (c).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
