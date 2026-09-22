# Non-backtracking random walk

↑ **Parent:** [Random walk on a graph](random-walk-on-a-graph.md)

A non-backtracking random walk remembers its preceding vertex and excludes that neighbor from the next choice. At vertices of degree at least two, it is a [Markov chain](markov-chain.md) on directed edges: $(a,b)$ moves to $(b,c)$ with probability $1/(\deg b-1)$ for each neighbor $c\ne a$. Dead ends require an additional convention. An initial vertex without a preceding edge uses the ordinary first-step neighbor distribution.

## ↑ Ancestors (9)

1. [Random walk on a graph](random-walk-on-a-graph.md)
2. [Random walk](random-walk.md)
3. [Markov chain](markov-chain.md)
4. [Markov process](markov-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Hitting a hub from two four-cycles](hitting-a-hub-from-two-four-cycles.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1/19h/solution.md)
