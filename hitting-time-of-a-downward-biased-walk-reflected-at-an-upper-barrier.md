# Hitting time of a downward-biased walk reflected at an upper barrier

↑ **Parent:** [Biased random walk](biased-random-walk.md)

On $\{0,\ldots,N\}$, stop at zero, move left with probability $q>1/2$ and right with probability $p=1-q$ at interior states, and move deterministically from $N$ to $N-1$. For $m_i=\mathbb E_iT_0$, the [first-step analysis](first-step-analysis.md) gives $m_0=0$, $m_i=1+qm_{i-1}+pm_{i+1}$ and $m_N=1+m_{N-1}$. Setting $D_i=m_i-m_{i-1}$ gives $qD_i-pD_{i+1}=1$, $D_N=1$, hence $D_i=[1-2p(p/q)^{N-i}]/(q-p)$. Summing these differences proves the displayed formula, and more generally $m_i=i/(q-p)-2pq(p/q)^{N-i}[1-(p/q)^i]/(q-p)^2$. A downward block has a uniformly positive probability of reaching zero, which supplies a geometric tail bound and justifies finiteness of these expectations.

## ↑ Ancestors (11)

1. [Biased random walk](biased-random-walk.md)
2. [Simple random walk on the integer line](simple-random-walk-on-the-integer-line.md)
3. [Random walk on a graph](random-walk-on-a-graph.md)
4. [Random walk](random-walk-split.md)
5. [Markov chain](markov-chain-split.md)
6. [Markov process](markov-process-split.md)
7. [Probability theory](probability-theory-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101/3/c/solution.md)
