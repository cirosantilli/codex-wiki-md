# Finite-population exclusion of permanent ALOHA collisions

↑ **Parent:** [Slotted ALOHA](slotted-aloha.md)

If a finite-population [slotted ALOHA](slotted-aloha.md) system has at most $M$ packets eligible to retry, uses independent retry probability $0<p<1$, and has conditional probability at least $\delta>0$ of no fresh attempts in any slot, then its conditional idle probability is at least $\delta(1-p)^M$. The probability that the next $k$ slots all collide is therefore at most $[1-\delta(1-p)^M]^k$. Letting $k\to\infty$ and taking a countable union over starting slots excludes eventual permanent collisions. Positive lower bounds on idle probability are essential: deterministic retries at probability one can create an absorbing collision state.

## ↑ Ancestors (9)

1. [Slotted ALOHA](slotted-aloha.md)
2. [Random access network](random-access-network.md)
3. [Stochastic network](stochastic-network.md)
4. [Queueing theory](queueing-theory-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-73/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35/3/solution.md)
