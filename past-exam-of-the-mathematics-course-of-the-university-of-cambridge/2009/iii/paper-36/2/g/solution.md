<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The [WinBUGS](../../../../../../winbugs.md) model uses a finite truncation of the reciprocal [prior](../../../../../../prior-probability.md). The numbered lines have the following roles:

- Line (1) forms $p_j=(1/j)/H_{5000}$, the normalized prior probability vector on the integer labels $1,\ldots,5000$. The deterministic sum may be declared after its use because the model is declarative.
- Line (2) assigns $N$ that [categorical distribution](../../../../../../categorical-distribution.md). The following observation model treats the supplied value $y=100$ as observed data, rather than as an unknown parameter.
- Line (3) forms observation probabilities $p[j]=1/N$ for $j\leq N$ and zero for $j>N$. For integer $N,j$, the small positive offset in `step(N-j+0.01)` includes the endpoint $j=N$ without depending on the convention at zero. There are exactly $N$ nonzero entries, so this vector sums to one.

Combining that [categorical distribution](../../../../../../categorical-distribution.md) observation likelihood with the truncated reciprocal [prior](../../../../../../prior-probability.md) produces

$$
\boxed{p(N\mid y)\propto N^{-2}\mathbf1_{\{y\leq N\leq5000\}}.}
$$

The [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md) output approximates this posterior. The actual PDF separates the observation line from the preceding comment; it must remain an active stochastic statement.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
