# Nearly-zero-sum pruning

↑ **Parent:** [Max-n search](max-n-search.md)

Suppose every terminal pair satisfies $|U_A+U_B|\le\epsilon$. At a B-node with immediate A-parent, let $\alpha$ be the A-coordinate of a completed alternative already retained by the parent. If a completed B-child supplies B-coordinate $y$, then every eventual B-selected pair $(u,v)$ has $v\ge y$ and hence $u\le\epsilon-y$. Therefore $\epsilon-y<\alpha$ permits discarding this B-option and skipping its remaining children. Equality is also safe if the parent keeps its existing option on a tie.

The inequality remains valid at completed subtrees because [max-n search](max-n-search.md) copies one terminal pair. If the observed pair is $(x,y)$, then $x+y\ge-\epsilon$, so $u\le x+2\epsilon$ and $x+2\epsilon\le\alpha$ is a weaker sufficient test. At $\epsilon=0$ this reduces to the usual MIN-node [alpha-beta pruning](alpha-beta-pruning.md) cutoff. A discarded option is not assigned a fabricated exact pair; the proof uses a certified alternative at the immediate parent.

## ↑ Ancestors (7)

1. [Max-n search](max-n-search.md)
2. [Game tree](game-tree.md)
3. [Game theory](game-theory-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/3/g/solution.md)
