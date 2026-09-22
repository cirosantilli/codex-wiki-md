<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Subtracting the two quadratic actions gives

$$
\log\frac{P_F}{P_B}
=-\frac1{2\sigma^2}
\int dt\,d\mathbf r
\left[
\left|\dot{\mathbf p}+\Gamma\frac{\delta F}{\delta\mathbf p}\right|^2
-\left|-\dot{\mathbf p}+\Gamma\frac{\delta F}{\delta\mathbf p}\right|^2
\right]
=-\frac{2\Gamma}{\sigma^2}
\int dt\,d\mathbf r\,
\dot{\mathbf p}\mathbin\cdot\frac{\delta F}{\delta\mathbf p}.
$$

The [functional chain rule](../../../../../../functional-chain-rule.md) identifies the last integral as $F_2-F_1$, so

$$
\frac{P_F}{P_B}
=\exp\left[-\frac{2\Gamma}{\sigma^2}(F_2-F_1)\right].
$$

Microscopic time-reversal invariance implies [detailed balance](../../../../../../detailed-balance.md). The equilibrium probability density of a configuration with free energy $F$ obeys

$$
P_{\rm eq}\mathrel\propto e^{-F/(k_BT)}.
$$

Therefore

$$
\frac{P_F}{P_B}
=\frac{e^{-F_2/(k_BT)}}{e^{-F_1/(k_BT)}}
=e^{-(F_2-F_1)/(k_BT)}.
$$

Comparison for arbitrary endpoint free energies yields the [Model A fluctuation-dissipation relation](../../../../../../model-a-fluctuation-dissipation-relation.md)

$$
\boxed{\sigma^2=2\Gamma k_BT.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
