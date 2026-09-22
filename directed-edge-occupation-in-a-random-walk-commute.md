# Directed edge occupation in a random-walk commute

↑ **Parent:** [Commute time identity](commute-time-identity.md)

Let [simple random walk](simple-random-walk.md) travel from $a\ne z$ to its first visit to $z$, then stop on its subsequent first hit of $a$ in a finite connected unweighted loopless [graph](graph-split.md). Every directed [edge](edge-of-a-graph.md) $u\to v$ has expected traversal count

$$
\mathbb E S(u,v)=R_{\mathrm{eff}}(a,z).
$$

The [Strong Markov property](strong-markov-property.md) splits the count into the two killed legs. By [killed-walk occupation voltage](killed-walk-occupation-voltage.md), their contributions are $v_{az}(u)$ and $v_{za}(u)$. Their Laplacians cancel, so the [harmonic maximum principle on a finite graph](harmonic-maximum-principle-on-a-finite-graph.md) makes the sum constant, with value $v_{az}(a)+v_{za}(a)=R_{\mathrm{eff}}(a,z)$. Summing over all directed [edges](edge-of-a-graph.md) recovers the [commute time identity](commute-time-identity.md).

## ↑ Ancestors (13)

1. [Commute time identity](commute-time-identity.md)
2. [Effective resistance](effective-resistance.md)
3. [Electrical network](electrical-network.md)
4. [Weighted graph](weighted-graph.md)
5. [Random walk on a graph](random-walk-on-a-graph.md)
6. [Random walk](random-walk.md)
7. [Markov chain](markov-chain.md)
8. [Markov process](markov-process-split.md)
9. [Probability theory](probability-theory-split.md)
10. [Probability and statistics](probability-and-statistics-split.md)
11. [Area of mathematics](area-of-mathematics.md)
12. [Mathematics](mathematics-split.md)
13. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/3/c/solution.md)
