# Exchangeable invariant events are tail events modulo null sets

↑ **Parent:** [Invariant sigma-algebra of an exchangeable sequence](invariant-sigma-algebra-of-an-exchangeable-sequence.md)

For a real sequence of [exchangeable random variables](exchangeable-random-variables.md), every event $A$ in its [invariant sigma-algebra of an exchangeable sequence](invariant-sigma-algebra-of-an-exchangeable-sequence.md) agrees almost surely with an event of its [tail sigma-algebra](tail-sigma-algebra.md). Put $F=\mathbf1_A$. Approximate $F$ in $L^1$ by its [conditional expectation](conditional-expectation.md) on the first $n+1$ coordinates. Swap that block with the next $n+1$ coordinates. Invariance of $A$ and the law shows that the conditional expectation on the second block is an equally good approximation. It is measurable with respect to the tail after index $n$. The [L1 contraction of conditional expectation](l1-contraction-of-conditional-expectation.md) then bounds $\|F-\mathbb E[F\mid\mathcal G_n]\|_1$ by twice the approximation error. The [reverse martingale convergence theorem](reverse-martingale-convergence-theorem.md) gives $F=\mathbb E[F\mid\bigcap_n\mathcal G_n]$ almost surely. Thresholding the latter at $1/2$ supplies the required tail event. Together with the reverse inclusion, the two sigma-algebras have identical probability completions.

## ↑ Ancestors (9)

1. [Invariant sigma-algebra of an exchangeable sequence](invariant-sigma-algebra-of-an-exchangeable-sequence.md)
2. [Exchangeable random variables](exchangeable-random-variables.md)
3. [Joint probability distribution](joint-probability-distribution.md)
4. [Probability distribution](probability-distribution.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Invariant sigma-algebra of an exchangeable sequence](invariant-sigma-algebra-of-an-exchangeable-sequence.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/3/b/solution.md)
