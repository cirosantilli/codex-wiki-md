<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [no unmeasured confounding assumption](../../../../../../conditional-exchangeability.md), or [conditional exchangeability](../../../../../../conditional-exchangeability.md), is

$$
(Y(0),Y(1))\mathrel\perp A\mid X.
$$

Also assume [consistency of potential outcomes](../../../../../../consistency-in-causal-inference.md), no [interference in causal inference](../../../../../../interference-in-causal-inference.md), [positivity in causal inference](../../../../../../positivity-assumption.md), and finite expectations. For $a\in\{0,1\}$, the [law of total expectation](../../../../../../law-of-total-expectation.md), exchangeability, and consistency give

$$
\begin{aligned}
\mathbb E[Y(a)]
&=\mathbb E\{\mathbb E[Y(a)\mid X]\}\\
&=\mathbb E\{\mathbb E[Y(a)\mid A=a,X]\}\\
&=\mathbb E\{\mathbb E[Y\mid A=a,X]\}.
\end{aligned}
$$

Positivity ensures that the observed conditional means exist on the covariate support being averaged. Subtracting the two cases identifies the [average treatment effect](../../../../../../average-treatment-effect.md) as

$$
\boxed{\beta_1
=\mathbb E\{\mathbb E[Y\mid A=1,X]\}
-\mathbb E\{\mathbb E[Y\mid A=0,X]\}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
