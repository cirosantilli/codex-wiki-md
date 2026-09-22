# Branching process conditioned on extinction

↑ **Parent:** [Galton-Watson process](galton-watson-process.md)

Let $q\in(0,1]$ be the [branching extinction probability](extinction-probability-of-a-branching-process.md) of a [Galton-Watson process](galton-watson-process.md) with offspring [probability generating function](probability-generating-function.md) $f$. Conditional on extinction, the probability of $j$ children is multiplied by $q^j/q$: every child's descendants must also become extinct. Hence the new [probability generating function](probability-generating-function.md) is $f_q$ and its mean is $f'(q)$. If $f'(q)<1$, the [total progeny of a branching process](total-progeny-of-a-branching-process.md) has conditional [expected value](expected-value.md) $1/(1-f'(q))$, and unconditionally $\mathbb E[T;T<\infty]=q/(1-f'(q))$. The [Markov inequality](markov-inequality.md) gives a finite-total-progeny tail bound without discarding the survival mass.

## ↑ Ancestors (5)

1. [Galton-Watson process](galton-watson-process.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Barely-supercritical largest-component expectation](barely-supercritical-largest-component-expectation.md)
- [Extinction probability of a branching process](extinction-probability-of-a-branching-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/4/ii/solution.md)
