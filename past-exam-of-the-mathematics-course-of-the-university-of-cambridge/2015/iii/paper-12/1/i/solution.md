<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $Z$ be a real [random variable](../../../../../../random-variable-split.md) with finite [expectation](../../../../../../expected-value.md) $m$ and finite [variance](../../../../../../variance-split.md) $\sigma^2$. **The [Chebyshev inequality](../../../../../../chebyshev-inequality.md) is**

$$
\boxed{\mathbb P(|Z-m|\geq t)\leq\frac{\sigma^2}{t^2}\quad(t>0).}
$$

The proof is the pointwise comparison

$$
t^2\mathbf1_{\{|Z-m|\geq t\}}\leq(Z-m)^2.
$$

Taking [expectations](../../../../../../expected-value.md) and using the definition of [variance](../../../../../../variance-split.md) gives

$$
t^2\mathbb P(|Z-m|\geq t)\leq\mathbb E(Z-m)^2=\sigma^2.
$$

Division by the positive number $t^2$ proves the [Chebyshev inequality](../../../../../../chebyshev-inequality.md), including the case $\sigma^2=0$. Equivalently, this is the [Markov inequality](../../../../../../markov-inequality.md) applied to the nonnegative [random variable](../../../../../../random-variable-split.md) $(Z-m)^2$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
