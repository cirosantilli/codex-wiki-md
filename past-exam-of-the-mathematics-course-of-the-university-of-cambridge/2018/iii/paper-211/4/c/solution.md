<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking [expectations](../../../../../../expected-value.md) in the single-step [discrete Tanaka formula](../../../../../../discrete-tanaka-formula.md), the [martingale transform](../../../../../../martingale-transform.md) term vanishes because $f$ is bounded and $\mathcal F_T$-measurable. Hence

$$
C(T+1,K)-C(T,K)=\frac12\mathbb E[\mathbf1_{\{S_T=K\}}(S_{T+1}-S_T)^2].
$$

At a state with $p_K=\mathbb P(S_T=K)>0$, the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives $\mathbb E[S_{T+1}\mid S_T=K]=K$, so the conditional second [moment](../../../../../../moment.md) of the increment is $\sigma^2(T,K)$. Part (a) gives $p_K=C(T,K+1)-2C(T,K)+C(T,K-1)$. Combining these identities yields the [discrete Dupire equation](../../../../../../discrete-dupire-equation.md)

$$
\boxed{C(T+1,K)-C(T,K)=\frac12\sigma^2(T,K)\bigl(C(T,K+1)-2C(T,K)+C(T,K-1)\bigr).}
$$

**The conditional [variance](../../../../../../variance-split.md) needs a positive-probability conditioning state.** The bound $|K-S_0|\leq T$ does not guarantee $p_K>0$. If $p_K=0$, both the [call-price curvature](../../../../../../discrete-call-price-curvature.md) and the time increment above are zero; the equation can be extended by assigning an arbitrary finite value to $\sigma^2(T,K)$ at such a state, but its conditional [variance](../../../../../../variance-split.md) is not determined there.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
