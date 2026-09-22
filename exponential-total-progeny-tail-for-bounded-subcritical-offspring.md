# Exponential total progeny tail for bounded subcritical offspring

↑ **Parent:** [Total progeny of a branching process](total-progeny-of-a-branching-process.md)

If a [Galton-Watson process](galton-watson-process-split.md) starts from one ancestor and has [bounded](boundedness.md) nonnegative [integer](integer-split.md) offspring $Z$ with $\mathbb E Z<1$, its [total progeny](total-progeny-of-a-branching-process.md) $T$ obeys $\mathbb P(T>n)\leq e^{-cn}$ for some $c>0$ and all [integers](integer-split.md) $n\geq1$. Explore one individual at a time. The unexplored [queue](queue-queueing-theory.md) has size $1+\sum_{j=1}^t(Z_j-1)$ until its first hit of zero, whose [hitting time](first-passage-time.md) is $T$. Hence $T>n$ implies $\sum_{j=1}^n(Z_j-1)\geq0$. [Boundedness](boundedness.md) makes $M(\theta)=\mathbb E e^{\theta(Z-1)}$ finite near zero, with $M(0)=1$ and $M'(0)=\mathbb E Z-1<0$. Choose $\theta>0$ with $M(\theta)<1$. The exponential [Markov inequality](markov-s-inequality.md) gives the desired bound with $c=-\log M(\theta)$. The same proof works whenever the offspring law has an [exponential moment](exponential-moment.md) near zero, even without [boundedness](boundedness.md).

## ↑ Ancestors (6)

1. [Total progeny of a branching process](total-progeny-of-a-branching-process.md)
2. [Galton-Watson process](galton-watson-process-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2011/b/6/b/solution.md)
