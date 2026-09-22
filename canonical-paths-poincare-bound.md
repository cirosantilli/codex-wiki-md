# Canonical paths Poincare bound

↑ **Parent:** [Canonical paths comparison theorem](canonical-paths-comparison-theorem.md)

Choose a directed [path](continuous-path.md) $\eta_{xy}$ of positive-probability transitions for each ordered pair of states in a finite [reversible Markov chain](reversible-markov-chain.md). Write $Q(e)=\pi(u)P(u,v)$ for a directed [edge](edge-of-a-graph.md) $e=(u,v)$, and let $N_e(\eta)$ count its occurrences. Define

$$
\rho=\max_{e:Q(e)>0}\frac1{Q(e)}\sum_{x,y}\pi(x)\pi(y)|\eta_{xy}|N_e(\eta_{xy}).
$$

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) bounds $(f(x)-f(y))^2$ by $|\eta_{xy}|$ times the sum of squared differences along the [path](continuous-path.md). Multiply by $\pi(x)\pi(y)/2$, sum and interchange finite sums. The identity $\operatorname{Var}_\pi(f)=\frac12\sum_{x,y}\pi(x)\pi(y)(f(x)-f(y))^2$ proves the bound. This convention counts directed [edges](edge-of-a-graph.md) and retains the factor $1/2$ in the [Dirichlet form of a Markov chain](dirichlet-form-of-a-markov-chain.md).

**Table of contents**

- [Path congestion](path-congestion.md)

## ↑ Ancestors (10)

1. [Canonical paths comparison theorem](canonical-paths-comparison-theorem.md)
2. [Dirichlet form of a Markov chain](dirichlet-form-of-a-markov-chain.md)
3. [Reversible Markov chain](reversible-markov-chain.md)
4. [Markov chain](markov-chain.md)
5. [Markov process](markov-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Canonical paths for the weighted matching chain](canonical-paths-for-the-weighted-matching-chain.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/3/d/solution.md)
- [Path congestion](path-congestion.md)
