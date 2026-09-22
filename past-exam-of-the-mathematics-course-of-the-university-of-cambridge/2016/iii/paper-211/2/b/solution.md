<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed maturity $T$, define $b_t^T=\int_t^T\sigma(t,u)\,du$ and $I_t^T=\int_t^T f(t,u)\,du$. The [stochastic Fubini theorem](../../../../../../stochastic-fubini-theorem.md) and the moving lower endpoint give

$$
dI_t^T=
\left[-r_t+\int_t^T\sigma(t,u)\int_t^u\sigma(t,v)\,dv\,du\right]dt
+b_t^T\,dW_t
=\left[-r_t+\frac12(b_t^T)^2\right]dt+b_t^T\,dW_t.
$$

The factor $1/2$ is the integral over one of the two triangles in the square $[t,T]^2$. Applying the [Itô formula](../../../../../../ito-s-lemma.md) to $P(t,T)=e^{-I_t^T}$, its quadratic-variation correction cancels that factor:

$$
\frac{dP(t,T)}{P(t,T)}=r_t\,dt-b_t^T\,dW_t.
$$

Set $D_t=e^{-\int_0^t r_sds}$, the reciprocal of the [continuous-time bank account](../../../../../../continuous-time-bank-account.md). The [Itô product rule](../../../../../../ito-product-rule.md) then gives

$$
D_tP(t,T)=P(0,T)\exp\!\left[-\int_0^t b_s^T\,dW_s-\frac12\int_0^t(b_s^T)^2ds\right].
$$

If $|\sigma|\leq M$, then $|b_t^T|\leq MT$ on this finite horizon. The [Novikov condition](../../../../../../novikov-s-condition.md) holds, so this [stochastic exponential](../../../../../../doleans-dade-exponential.md) is a true [martingale](../../../../../../martingale-split.md), not merely a [local martingale](../../../../../../local-martingale.md). **The discounted price is therefore**

$$
\boxed{D_tP(t,T)\text{ is a }\mathbb Q\text{-martingale}.}
$$

The authoritative PDF discounts to $t$ in this part. The TeX transcription's upper endpoint $T$ would include future [short rates](../../../../../../short-rate.md) and is incorrect here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
