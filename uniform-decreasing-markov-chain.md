# Uniform decreasing Markov chain

↑ **Parent:** [Expected hitting time](expected-hitting-time.md)

On $\{1,\ldots,n\}$, make $1$ an [absorbing state](absorbing-state.md) and let each state $i>1$ move uniformly to $\{1,\ldots,i-1\}$. Its [expected hitting time](expected-hitting-time.md) of $1$, allowing zero time when started at $1$, is $e_i=H_{i-1}$. [First-step analysis](first-step-analysis.md) gives $e_i=1+(i-1)^{-1}\sum_{j<i}e_j$; subtracting consecutive recurrences yields $e_i-e_{i-1}=1/(i-1)$ and hence the formula.

## ↑ Ancestors (8)

1. [Expected hitting time](expected-hitting-time.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/20h/solution.md)
