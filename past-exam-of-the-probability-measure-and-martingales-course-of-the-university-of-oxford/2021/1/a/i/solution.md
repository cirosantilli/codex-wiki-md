<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $A=\{|X|\geq Z\}$. Both $A$ and its [indicator function](../../../../../indicator-function.md) are [measurable](../../../../../measurability.md), and $0\leq Z\mathbf1_A\leq |X|$. Thus $Z\mathbf1_A$ is an [integrable random variable](../../../../../integrable-random-variable.md). Monotonicity of [conditional expectation](../../../../../conditional-expectation.md) gives

$$
\mathbb E[Z\mathbf1_A\mid\mathcal G]\leq\mathbb E[|X|\mid\mathcal G]\quad\text{a.s.}
$$

The measurable-factor property of [conditional expectation](../../../../../conditional-expectation.md) says that a bounded $\mathcal G$-[measurable function](../../../../../measurable-function.md) $H$ satisfies $\mathbb E[HW\mid\mathcal G]=H\mathbb E[W\mid\mathcal G]$ for every [integrable random variable](../../../../../integrable-random-variable.md) $W$. Here the factor $Z$ need not be bounded. Apply that property first to $Z\wedge m$ and $W=\mathbf1_A$, then use [monotone convergence](../../../../../monotone-convergence-theorem.md) on the nonnegative products, including the conditional version, to obtain

$$
\mathbb E[Z\mathbf1_A\mid\mathcal G]
=\lim_{m\to\infty}(Z\wedge m)\mathbb E[\mathbf1_A\mid\mathcal G]
=Z\mathbb E[\mathbf1_A\mid\mathcal G].
$$

All the left-hand [conditional expectations](../../../../../conditional-expectation.md) are well defined; the final one is finite [almost surely](../../../../../almost-sure-convergence.md) because $Z\mathbf1_A$ is an [integrable random variable](../../../../../integrable-random-variable.md). Since $Z>0$ [almost surely](../../../../../almost-sure-convergence.md), division now yields

$$
\boxed{\mathbb E[\mathbf1_{\{|X|\geq Z\}}\mid\mathcal G]
\leq Z^{-1}\mathbb E[|X|\mid\mathcal G]\quad\text{a.s.}}
$$

This proves the [conditional Markov inequality with a measurable threshold](../../../../../conditional-markov-inequality-with-a-measurable-threshold.md) without assuming that $Z^{-1}|X|$ is an [integrable random variable](../../../../../integrable-random-variable.md). The measurable-factor rule, with its product-integrability condition, is also stated in the standard [conditional expectation](../../../../../conditional-expectation.md) theory.[§4.1.2, Theorem 4.1.14, printed pp. 212–213: bringing out a measurable factor](../../../../../probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
