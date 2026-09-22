# Labelled bicyclic graph count

↑ **Parent:** [Bicyclic graph](bicyclic-graph.md)

If $b_k$ counts labelled bicyclic cores on $k$ vertices, the [bicyclic kernel classification](bicyclic-kernel-classification.md) gives $b_k\leq A k!k^2$. Three internally nonempty paths between two branching vertices give $b_k\geq k!\binom{k-3}{2}/12$ for $k\geq5$. Attach a forest with those core vertices as roots to obtain $C(n,n+1)=\sum_k\binom nk b_kkn^{n-k-1}$. After division by $n^{n+1}$ the relevant sum is $n^{-2}\sum_k k^3(n)_k/n^k$. Its upper bound follows from $(n)_k/n^k\leq e^{-k(k-1)/(2n)}$; its lower bound uses $\sqrt n\leq k\leq2\sqrt n$, where this product stays bounded below. The sum is bounded above and below by positive constants. The restriction $n\geq4$ is necessary: $C(3,4)=0$.

## ↑ Ancestors (7)

1. [Bicyclic graph](bicyclic-graph.md)
2. [Graph excess](graph-excess.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/4/ii/solution.md)
