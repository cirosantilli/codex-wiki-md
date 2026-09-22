# Consecutive-clearance inspection model

↑ **Parent:** [Two-phase inspection model](two-phase-inspection-model.md)

In the [consecutive-clearance inspection model](consecutive-clearance-inspection-model.md), a run of $K$ consecutive good items is required to leave full inspection. With $q=1-p$, $0<p<1$, its [Markov chain](markov-chain-split.md) has transitions $P_{i0}=p$, $P_{i,i+1}=q$ for $i<K$, and $P_{K0}=p/r$, $P_{KK}=1-p/r$. Thus every defect in the clearance phase resets the count, rather than preserving the cumulative total.

Writing $D=1+(r-1)q^K$, the [stationary distribution](stationary-distribution.md) is

$$
\pi_i=\frac{pq^i}{D}\quad(0\leq i<K),\qquad\pi_K=\frac{rq^K}{D}.
$$

To prove this, balance at $i=1,\ldots,K-1$ gives $\pi_i=q^i\pi_0$, while balance at $K$ gives $(p/r)\pi_K=q^K\pi_0$. Summing the geometric series and normalizing gives $\pi_0=p/D$; balance at zero follows as well. The inspected fraction is $1-(1-1/r)\pi_K=1/D$. The fraction of all production that is both defective and uninspected is $p(r-1)q^K/D$; the fraction among defective items alone is $(r-1)q^K/D$. All these long-run limits follow from the [Markov chain ergodic theorem](markov-chain-ergodic-theorem.md) and the independent inspection coins. The distinction from cumulative clearance matters already at $K=2$.

## ↑ Ancestors (8)

1. [Two-phase inspection model](two-phase-inspection-model.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Consecutive-clearance inspection model](consecutive-clearance-inspection-model.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2004/n/n2/b/i/solution.md)
- [Two-phase inspection model](two-phase-inspection-model.md)
