# Conditional Markov inequality with a measurable threshold

↑ **Parent:** [Markov's inequality](markov-s-inequality.md)

If $X$ is an [integrable random variable](integrable-random-variable.md) and $Z$ is a finite, strictly positive $\mathcal G$-[measurable](measurability.md) [random variable](random-variable-split.md), then

$$
\mathbb E[\mathbf1_{\{|X|\geq Z\}}\mid\mathcal G]
\leq\frac{\mathbb E[|X|\mid\mathcal G]}{Z}\quad\text{a.s.}
$$

Indeed, $0\leq Z\mathbf1_{\{|X|\geq Z\}}\leq|X|$. Monotonicity of [conditional expectation](conditional-expectation.md) and the [measurable-factor rule for conditional expectation](measurable-factor-rule-for-conditional-expectation.md) give

$$
Z\mathbb E[\mathbf1_{\{|X|\geq Z\}}\mid\mathcal G]
\leq\mathbb E[|X|\mid\mathcal G].
$$

Division by the strictly positive $Z$ proves the claim. Only the displayed product needs to be an [integrable random variable](integrable-random-variable.md); neither $Z$ nor $|X|/Z$ needs to have finite [expected value](expected-value-split.md). The measurable threshold represents information already available before asking how likely the remaining exceedance is.

## ↑ Ancestors (7)

1. [Markov's inequality](markov-s-inequality.md)
2. [Probability inequality](probability-inequality-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/1/a/i/solution.md)
