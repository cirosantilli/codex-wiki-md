# Total progeny with critical geometric offspring

↑ **Parent:** [Geometric-offspring critical branching process](geometric-offspring-critical-branching-process.md)

Start a [branching process](branching-process.md) with one ancestor and [offspring distribution](offspring-distribution-of-a-branching-process.md) $\mathbb P(N=k)=2^{-k-1}$ for $k\ge0$. Its [probability generating function](probability-generating-function.md) is $G_N(s)=1/(2-s)$ and its mean offspring count is $1$, making it a [critical branching process](critical-branching-process.md). Splitting the family at the ancestor gives the [total progeny](total-progeny-of-a-branching-process.md) recursion $Z=1+\sum_{i=1}^N Z_i$. The [probability generating function of an independent random sum](probability-generating-function-of-an-independent-random-sum.md) then gives $G_Z=s/(2-G_Z)$, whose root satisfying $G_Z(0)=0$ is $1-\sqrt{1-s}$. Its limit at $s\uparrow1$ equals $1$, consistent with finite [total progeny](total-progeny-of-a-branching-process.md) almost surely; its [derivative](derivative.md) diverges there, so the [expectation](expected-value-split.md) of $Z$ is nevertheless infinite.

## ↑ Ancestors (6)

1. [Geometric-offspring critical branching process](geometric-offspring-critical-branching-process.md)
2. [Galton-Watson process](galton-watson-process-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/probability/8/b/iii/solution.md)
