# Measurable-factor rule for conditional expectation

↑ **Parent:** [Conditional expectation](conditional-expectation.md)

Let $Y$ be an [integrable random variable](integrable-random-variable.md), let $H$ be a finite $\mathcal G$-[measurable](measurability.md) [random variable](random-variable-split.md), and suppose $HY$ is an [integrable random variable](integrable-random-variable.md). Then a known factor can be taken outside the [conditional expectation](conditional-expectation.md):

$$
\mathbb E[HY\mid\mathcal G]=H\mathbb E[Y\mid\mathcal G]\quad\text{a.s.}
$$

For a bounded $H$, first verify the defining [integral](integral-split.md) identity when $H$ is the [indicator function](indicator-function.md) of a [measurable set](measurable-set.md) in $\mathcal G$, extend by [linearity](linearity.md) to [simple functions](simple-function.md), and then use bounded approximation and the [dominated convergence theorem](dominated-convergence-theorem.md). For nonnegative $H,Y$, truncating $H$ and using the [conditional monotone convergence theorem](conditional-monotone-convergence-theorem.md) proves the identity with extended nonnegative [conditional expectations](conditional-expectation.md). In particular,

$$
\mathbb E\bigl[|H|\mathbb E[|Y|\mid\mathcal G]\bigr]=\mathbb E|HY|<\infty.
$$

For general $H,Y$ under the stated [integrability](integrability.md) assumptions, the [conditional Jensen inequality](conditional-jensen-inequality.md) bounds $|H\mathbb E[Y\mid\mathcal G]|$ by that [integrable random variable](integrable-random-variable.md). Apply the bounded-factor result to truncations of $H$, then use the [dominated convergence theorem](dominated-convergence-theorem.md) on the products and the [L1 contraction of conditional expectation](l1-contraction-of-conditional-expectation.md). This proves the identity without assuming $H$ itself is an [integrable random variable](integrable-random-variable.md).

The product-integrability condition is essential to the ordinary finite [conditional expectation](conditional-expectation.md) statement. An unbounded factor cannot be moved through an [expected value](expected-value-split.md) simply because its partner is an [integrable random variable](integrable-random-variable.md).[§4.1.2, Theorem 4.1.14, printed pp. 212–213](probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

## ↑ Ancestors (7)

1. [Conditional expectation](conditional-expectation.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Conditional Markov inequality with a measurable threshold](conditional-markov-inequality-with-a-measurable-threshold.md)
- [Mutual conditional expectation rigidity in L2](mutual-conditional-expectation-rigidity-in-l2.md)
