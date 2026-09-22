<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This part's conditional-expectation representation is its own hypothesis; it does not need the incorrect unrestricted claim in part (b). Fix $T$, and write

$$
I_t(T)=\int_t^Tf_t(u)\,du,\qquad
\beta_t(T)=\int_t^TB_t(u)\,du,\qquad
M_t(T)=U_te^{-I_t(T)}.
$$

The assumed representation makes $M(T)$ a [martingale](../../../../../../martingale-split.md). The [stochastic Fubini theorem](../../../../../../stochastic-fubini-theorem.md) gives

$$
dI_t(T)=\left(\int_t^TA_t(u)\,du-f_t(t)\right)dt+\beta_t(T)\,dW_t.
$$

Apply the [Itô formula](../../../../../../ito-s-lemma.md) to $e^{-I}$ and use the equation for $U$ from part (a), including the cross-variation. The result is

$$
\frac{dM_t(T)}{M_t(T)}
=\left[f_t(t)-\frac18\sigma_t^2-\int_t^TA_t(u)\,du
+\frac12\beta_t(T)^2-\frac12\sigma_t\beta_t(T)\right]dt
+\left(\frac12\sigma_t-\beta_t(T)\right)dW_t.
$$

Uniqueness of the continuous [semimartingale](../../../../../../semimartingale.md) decomposition makes the drift vanish. Initially this is a $dt\,d\mathbb P$ statement; the assumed continuity in time and maturity extends it to the continuous versions simultaneously. Let $T\downarrow t$ to obtain

$$
\boxed{f_t(t)=\frac18\sigma_t^2=k\sigma_t^2.}
$$

Substitute back and differentiate the maturity integrals using their continuous integrands:

$$
\boxed{A_t(T)=B_t(T)\left(\int_t^TB_t(u)\,du-\frac12\sigma_t\right).}
$$

This is the [forward drift restriction for square-root stock claims](../../../../../../forward-drift-restriction-for-square-root-stock-claims.md). The $-\sigma_t/2$ term comes from the product cross-variation and must be retained. For the uninformative zero-[stock](../../../../../../stock.md) case, the representation does not identify $f$; as usual a positive initial [stock](../../../../../../stock.md) price is understood.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
