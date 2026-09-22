# Expected query cost

↑ **Parent:** [Decision-tree query cost](decision-tree-query-cost.md)

For a fixed [decision tree](decision-tree.md) $T$ and [input](input-computer-science.md) [probability distribution](probability-distribution-split.md) $\mu$, its [expected query cost](expected-query-cost.md) is

$$
\mathbb E_\mu[q_T(X)]=\sum_{x\in\{0,1\}^n}\mu(x)q_T(x).
$$

Under the [discrete uniform distribution](discrete-uniform-distribution.md) on the eight three-[bit](bit.md) [inputs](input-computer-science.md), the [three-bit majority decision tree](three-bit-majority-decision-tree.md) has

$$
\Pr(q_T(X)=2)=\Pr(q_T(X)=3)=\frac12,\qquad \mathbb E[q_T(X)]=2\cdot\frac12+3\cdot\frac12=\frac52=2.5.
$$

This is an exact average, not a fractional query made during one execution. It is also optimal among exact deterministic [decision trees](decision-tree.md) under this [discrete uniform distribution](discrete-uniform-distribution.md): one observed [bit](bit.md) never determines the [majority function](majority-function.md); whichever two distinct coordinates are inspected first, their values disagree with [probability](probability.md) $1/2$, forcing a third query. In comparison, querying all three [bits](bit.md) unconditionally has the same actual depth three but [expected query cost](expected-query-cost.md) three.

For an arbitrary [input](input-computer-science.md) [probability distribution](probability-distribution-split.md), the same fixed [three-bit majority decision tree](three-bit-majority-decision-tree.md) gives $\mathbb E_\mu[q_T(X)]=2+\Pr_\mu(X_1\ne X_2)$. For three [independent random variables](independent-random-variables.md), each a [Bernoulli random variable](bernoulli-distribution.md) with common one-[probability](probability.md) $p$, this becomes $2+2p(1-p)$; the value $2.5$ depends on $p=1/2$. Averaging over [inputs](input-computer-science.md) should also be distinguished from averaging over an algorithm's internal random choices at a fixed [input](input-computer-science.md).[O'Donnell, Saks, Schramm and Servedio, Every decision tree has an influential variable, sections 1.1–1.2, pp. 1–2: worst-input expected randomized cost R(f) versus input-distribution average Δ(T)](every-decision-tree-has-an-influential-variable-by-ryan-o-donnell-and-others.md)

## ↑ Ancestors (7)

1. [Decision-tree query cost](decision-tree-query-cost.md)
2. [Decision tree](decision-tree.md)
3. [Decision tree model](decision-tree-model.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Coordinate revealment](coordinate-revealment.md)
- [Decision-tree depth](decision-tree-depth.md)
- [Decision-tree query cost](decision-tree-query-cost.md)
- [Expected query cost](expected-query-cost.md)
- [Parity lower bound for Boolean queries](parity-lower-bound-for-boolean-queries.md)
