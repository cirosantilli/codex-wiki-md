# Binomial branching process conditioned on extinction

↑ **Parent:** [Branching process conditioned on extinction](branching-process-conditioned-on-extinction.md)

For offspring $\operatorname{Bin}(k,p)$ with $0<p<1$ and $kp>1$, let $\eta\in(0,1)$ be the [branching extinction probability](extinction-probability-of-a-branching-process.md). Conditioning on [extinction](extinction.md) changes the offspring law to $\operatorname{Bin}(k,\widetilde p)$ with the displayed parameter. Indeed, the [probability](probability.md) of $j$ children is multiplied by $\eta^{j-1}$, so the new [probability generating function](probability-generating-function.md) is $f(\eta s)/\eta$. Since $f(s)=(1-p+ps)^k$ and $f(\eta)=\eta$, this equals $((1-p+p\eta s)/(1-p+p\eta))^k$. Its [mean](expected-value-split.md) is $k\widetilde p=f'(\eta)<1$, because [strict convexity](strictly-convex-function.md) of $f(s)-s$ and its zeros at $\eta$ and one force a negative [derivative](derivative.md) at the smaller zero. The conditioned process therefore has an exponentially decaying total-progeny tail. Unconditionally that tail instead converges to the survival mass $1-\eta$, with an exponentially small correction. When [extinction](extinction.md) has [probability](probability.md) zero, conditioning on it does not define this law.

## ↑ Ancestors (6)

1. [Branching process conditioned on extinction](branching-process-conditioned-on-extinction.md)
2. [Galton-Watson process](galton-watson-process-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2011/b/6/c/solution.md)
