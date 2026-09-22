<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For a specified field trajectory, the required normalized noise is

$$
\boldsymbol\Lambda_F
=\frac{\dot{\mathbf p}
+\Gamma\,\delta F/\delta\mathbf p-\Gamma\mathbf Y}
{\sqrt{2k_BT\Gamma}},
$$

and time reversal changes only $\dot{\mathbf p}$ to $-\dot{\mathbf p}$. Assuming equal additive-noise Jacobians, the difference of the two [Onsager--Machlup actions](../../../../../../onsager-machlup-path-probability-for-model-a-dynamics.md) gives

$$
\log\frac{\mathbb P_F}{\mathbb P_B}
=-\beta\int_{t_1}^{t_2}dt\int d\mathbf r\,
\dot{\mathbf p}\mathbin\cdot
\left(\frac{\delta F}{\delta\mathbf p}-\mathbf Y\right).
$$

The [functional chain rule](../../../../../../functional-chain-rule.md) identifies the first term as $-\beta\Delta F$, so

$$
\boxed{\frac{\mathbb P_F[\mathbf p]}{\mathbb P_B[\mathbf p]}
=\exp\left[
-\beta\Delta F
+\beta\int_{t_1}^{t_2}dt\int d\mathbf r\,
\mathbf Y\mathbin\cdot\dot{\mathbf p}
\right].}
$$

The forcing performs generalized work $W_Y=\int\mathbf Y\cdot\dot{\mathbf p}$, and $W_Y-\Delta F$ is the heat dissipated into the bath. The formula is therefore the field-theory form of [local detailed balance](../../../../../../local-detailed-balance.md) and quantifies nonequilibrium entropy production.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
