# Weak PAC learning

↑ **Parent:** [Statistical learning theory](statistical-learning-theory.md)

A [concept class](concept-class.md) $C$ is weakly PAC learnable using a [hypothesis class](concept-class.md) $H$ when a learning procedure has a fixed edge $\gamma>0$ such that, for every target in $C$, every input [probability distribution](probability-distribution-split.md), and every confidence parameter $\delta$, sufficiently many independent target-labelled examples let it return an $h\in H$ satisfying the displayed bound with probability at least $1-\delta$. The example bound must be polynomial in $1/\delta$ under this definition. Computational efficiency is an additional requirement when explicitly imposed. This distribution-wide guarantee should be distinguished from merely obtaining an advantage on one finite training sample.

## ↑ Ancestors (5)

1. [Statistical learning theory](statistical-learning-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-learning-theory/3/a/solution.md)
- [Two-interval approximation by one interval](two-interval-approximation-by-one-interval.md)
