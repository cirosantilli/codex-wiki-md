# Gaussian smoothing of an integer-valued distribution

↑ **Parent:** [Convolution of independent random variables](convolution-of-independent-random-variables.md)

Let $X$ take integer values with probabilities $p_n$, and let $Y_\sigma$ be an independent centered [normal distribution](normal-distribution.md) with positive [standard deviation](standard-deviation.md) $\sigma$. Conditioning on $X$ gives the [probability density function](probability-density-function.md) of their sum as $g_\sigma(z)=\sum_np_n\varphi_\sigma(z-n)$, where $\varphi_\sigma$ is the normal density. Nonnegativity and [Tonelli's theorem](tonelli-theorem.md) show that this density integrates to one. For small $\sigma$, isolated atoms become narrow smooth peaks with their original probability masses.

For each fixed real $t$, [dominated convergence](dominated-convergence-theorem.md) gives

$$
\sigma g_\sigma(\sigma t)=\mathbb E\varphi_1(t-X/\sigma)\longrightarrow\varphi_1(t)\qquad(\sigma\to\infty),
$$

since $X/\sigma\to0$ almost surely and $\varphi_1$ is bounded. Thus every fixed integer-valued distribution acquires a Gaussian central profile on this expanding scale, without any moment assumption on $X$. This is not a claim about uniform relative error in the tails or about finite moments. For example, if $p_n=3/(\pi^2n^2)$ for $n\ne0$ and $p_0=0$, the [expectation](expected-value-split.md) of $|X|$ is infinite. Since $\mathbb E|Y_\sigma|<\infty$, the triangle inequality forces $\mathbb E|X+Y_\sigma|=\infty$ too. Symmetry then gives equal infinite positive and negative first moments, so there is no ordinary mean. The second moment is also infinite. A Gaussian-looking center can therefore coexist with a [heavy-tailed distribution](heavy-tailed-distribution.md).

## ↑ Ancestors (8)

1. [Convolution of independent random variables](convolution-of-independent-random-variables.md)
2. [Joint probability distribution](joint-probability-distribution.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1/15/b/solution.md)
