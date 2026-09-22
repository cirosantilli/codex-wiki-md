<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The square root is concave on $[0,\infty)$, and $\sqrt{S_T}$ is [integrable](../../../../../../integrability.md) since $\mathbb E\sqrt{S_T}\leq\sqrt{\mathbb ES_T}$. For $t\leq T_1\leq T_2$, the [conditional Jensen inequality](../../../../../../conditional-jensen-inequality.md) and the [martingale](../../../../../../martingale-split.md) property give

$$
\mathbb E[\sqrt{S_{T_2}}\mid\mathcal F_{T_1}]
\leq\sqrt{\mathbb E[S_{T_2}\mid\mathcal F_{T_1}]}
=\sqrt{S_{T_1}}.
$$

Taking [conditional expectations](../../../../../../conditional-expectation.md) with respect to $\mathcal F_t$ and using the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) yields

$$
\boxed{C(t,T_2)\leq C(t,T_1)\quad\text{almost surely}.}
$$

Thus the maturity curve for a [square-root stock claim](../../../../../../square-root-stock-claim.md) is nonincreasing; it need not be strictly decreasing, as a constant stock gives equality. The inequality holds for every ordered pair of maturities. Under the usual right-continuous versions of the market processes, it gives the corresponding nonincreasing version of the maturity curve.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
