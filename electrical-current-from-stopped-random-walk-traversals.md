# Electrical current from stopped random-walk traversals

↑ **Parent:** [Electrical network](electrical-network.md)

In a finite connected [electrical network](electrical-network.md), run the conductance [random walk](random-walk.md) from $s$ until its first visit to a distinct vertex $t$. Let $G(s,x)$ be the expected visits to $x$ before stopping, and $w_x=\sum_yw_{xy}$. The expected signed number of traversals of $\{x,y\}$ is the displayed expression. Its divergence is $\mathbf1_{x=s}-\mathbf1_{x=t}$ by telescoping each path, and its resistance-weighted sum around a cycle is zero because $G(s,x)/w_x$ is a voltage. Uniqueness follows by summing $\sum_{\{x,y\}}w_{xy}(v_x-v_y)^2$: a zero-divergence voltage flow has zero energy. Thus the expected net traversals are exactly the unit source-to-sink current.

## ↑ Ancestors (11)

1. [Electrical network](electrical-network.md)
2. [Weighted graph](weighted-graph.md)
3. [Random walk on a graph](random-walk-on-a-graph.md)
4. [Random walk](random-walk.md)
5. [Markov chain](markov-chain.md)
6. [Markov process](markov-process-split.md)
7. [Probability theory](probability-theory-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-38/1/solution.md)
