# Linearity of integration

↑ **Parent:** [Integral](integral.md)

For [integrable](integrability.md) [real-valued functions](real-valued-function.md) $f,g$ on a [measure space](measure-space.md) $(X,\mu)$ and fixed [real numbers](real-number.md) $a,b$, their [linear combination](linear-combination.md) $af+bg$ is [integrable](integrability.md), and the [Lebesgue integral](lebesgue-integral.md) satisfies

$$
\int_X(af+bg)\,d\mu=a\int_X f\,d\mu+b\int_X g\,d\mu.
$$

The same rule applies to any finite [summation](summation.md): $\int_X\sum_{j=1}^n a_jf_j\,d\mu=\sum_{j=1}^n a_j\int_X f_j\,d\mu$ for [integrable](integrability.md) [functions](function-split.md) $f_j$ and fixed [scalars](scalar.md) $a_j$. Finite signed values matter: [integrability](integrability.md) ensures all these [integrals](integral.md) are finite, so no undefined $\infty-\infty$ occurs.

This is the [distributive property](distributive-property.md) of finite [summation](summation.md) carried into [integration](integral.md): a fixed factor can be pulled out, and a finite sum can be integrated term by term. For [simple functions](simple-function.md), distribute the finite sums of value times [measure](measure.md); approximation extends additivity to nonnegative [measurable functions](measurable-function.md), and splitting into a [positive part](positive-part-of-a-real-valued-function.md) and [negative part](negative-part-of-a-real-valued-function.md) gives the [integrable](integrability.md) signed case. See [Lecture 12: Lebesgue Integrable Functions, the Lebesgue Integral and the Dominated Convergence Theorem](18-102-introduction-to-functional-analysis-spring-2021-lecture-notes-by-andrew-lin/lecture-12-lebesgue-integrable-functions-the-lebesgue-integral-and-the-dominated-convergence-theorem.md) (Proposition 122: linearity for integrable functions). For example, $\int_0^1(2x-3)\,dx=2\int_0^1x\,dx-3\int_0^1 1\,dx=-2$. With a [probability measure](probability-measure.md), [linearity of integration](linearity-of-integration.md) gives [linearity of expectation](linearity-of-expectation.md).

## ↑ Ancestors (7)

1. [Integral](integral.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Linearity of expectation](linearity-of-expectation.md)
- [Linearity of integration](linearity-of-integration.md)
- [Signed area under a graph](signed-area-under-a-graph.md)
- [Wavelet polynomial annihilation](wavelet-polynomial-annihilation.md)
