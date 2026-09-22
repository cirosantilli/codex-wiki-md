<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Set the noise strengths to the [model A fluctuation-dissipation relation](../../../../../../model-a-fluctuation-dissipation-relation.md) and the [fluctuation-dissipation relation for a conserved flux](../../../../../../fluctuation-dissipation-relation-for-a-conserved-flux.md):

$$
\sigma^2=2\Gamma k_BT,\qquad\sigma_N^2=2Mk_BT.
$$

The preceding logarithmic ratio becomes

$$
\log\frac{P_F}{P_B}=-\frac1{k_BT}\int[\mu_j\dot p_j+\mu_j\partial_iW_{ij}+W_{ij}\partial_i\mu_j].
$$

The last two terms combine as $\partial_i(\mu_jW_{ij})$. They integrate to zero under the periodic [boundary conditions](../../../../../../boundary-condition.md), by [integration by parts](../../../../../../integration-by-parts.md). The remaining term is $F_2-F_1$ by the [functional chain rule](../../../../../../functional-chain-rule.md), hence

$$
\boxed{\frac{P_F}{P_B}=e^{-(F_2-F_1)/(k_BT)}.}
$$

After including the equilibrium initial weights, the forward and reversed histories have equal probability. Thus [microscopic reversibility](../../../../../../microscopic-reversibility.md) is satisfied by the two channels together, with each channel's own thermal noise strength.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
