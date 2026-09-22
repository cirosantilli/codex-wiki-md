# Two-phase inspection model

↑ **Parent:** [Markov chain](markov-chain-split.md)

A [two-phase inspection model](two-phase-inspection-model.md) alternates between inspecting every item and inspecting each item with [probability](probability.md) $1/r$, where $r>1$. Suppose item defects are independent with probability $p\in(0,1)$. The first phase ends after $K\geq1$ good items have been accumulated, while the second ends upon detecting a defect. With state $i<K$ equal to the cumulative number of good items found during the current full-inspection phase, the [Markov chain](markov-chain-split.md) has transitions $P_{ii}=p$, $P_{i,i+1}=q=1-p$, $P_{K0}=p/r$, $P_{KK}=1-p/r$.

Its [stationary distribution](stationary-distribution.md) is $\pi_i=p/(Kp+rq)$ for $i<K$ and $\pi_K=rq/(Kp+rq)$. Indeed, balance gives equal mass to every phase-A state and $p\pi_K/r=q\pi_{K-1}$; normalization fixes the common mass. The finite chain is irreducible and aperiodic, so the [Markov chain ergodic theorem](markov-chain-ergodic-theorem.md) identifies these probabilities with long-run occupation fractions. The long-run inspected fraction is $1-(1-1/r)\pi_K=(Kp+q)/(Kp+rq)$. The fraction of all production consisting of undetected defective items is $p(1-1/r)\pi_K=p(r-1)q/(Kp+rq)$.

An important modeling choice is whether defects during full inspection preserve accumulated good items or reset the count. Resetting produces the distinct [consecutive-clearance inspection model](consecutive-clearance-inspection-model.md) and changes the long-run fractions.

**Table of contents**

- [Consecutive-clearance inspection model](consecutive-clearance-inspection-model.md)

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Two-phase inspection model](two-phase-inspection-model.md)
