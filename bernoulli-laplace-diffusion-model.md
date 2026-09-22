# Bernoulli-Laplace diffusion model

↑ **Parent:** [Markov chain](markov-chain-split.md)

Two urns each contain $n$ balls, with $n$ red and $n$ blue balls in total. Independently choose one ball uniformly from each urn and exchange them. The red count $R_k$ in the first urn is a [Markov chain](markov-chain-split.md) on $\{0,\ldots,n\}$. Its upward and downward probabilities are displayed above, and the probability of remaining at $r$ is $2r(n-r)/n^2$. Thus $\mathbb E[R_{k+1}\mid R_k=r]=1+(1-2/n)r$. Starting from $R_0=n$, [linearity of expectation](linearity-of-expectation.md) gives $\mathbb E[R_k]=n/2+(n/2)(1-2/n)^k$, with the initial value separately understood when $n=2,k=0$. Random exchanges drive the expected imbalance toward zero.

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2023/prelims/mathematics-iii/4/b/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/7/b/ii/solution.md)
