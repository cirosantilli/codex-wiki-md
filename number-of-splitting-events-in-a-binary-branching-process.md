# Number of splitting events in a binary branching process

↑ **Parent:** [Total progeny of a branching process](total-progeny-of-a-branching-process.md)

Consider a [Galton-Watson process](galton-watson-process-split.md) started by one individual, with offspring count $2$ with [probability](probability.md) $p<1/2$ and $0$ with [probability](probability.md) $q=1-p$. Let $N$ count individuals producing two offspring. At the first generation, either $N=0$, or $N=1+N_1+N_2$ for independent copies $N_1,N_2$. Its [probability generating function](probability-generating-function.md) therefore satisfies $G=q+psG^2$ and

$$
G(s)=\frac{2q}{1+\sqrt{1-4pqs}}.
$$

The branch is fixed by $G(0)=q$. Differentiation at $s=1$ gives $\mathbb E[N]=p/(1-2p)$. Alternatively, generation $t$ has expected size $(2p)^t$, so its expected splitting count is $p(2p)^t$ and summing gives the same result. The total progeny is $2N+1$, since every split creates two new individuals.

## ↑ Ancestors (6)

1. [Total progeny of a branching process](total-progeny-of-a-branching-process.md)
2. [Galton-Watson process](galton-watson-process-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability/8/b/ii/solution.md)
