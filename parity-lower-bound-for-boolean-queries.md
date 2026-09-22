# Parity lower bound for Boolean queries

↑ **Parent:** [Decision tree](decision-tree.md)

For three [bits](bit.md), the [Boolean function](boolean-function.md) $p(x)=x_1\mathbin\oplus x_2\mathbin\oplus x_3$ outputs one when $x_1+x_2+x_3$ is odd, where $\oplus$ denotes [exclusive or](exclusive-or.md). Unlike the [three-bit majority decision tree](three-bit-majority-decision-tree.md), an exact [decision tree](decision-tree.md) computing [parity](parity.md) must inspect all three [bits](bit.md) on every [input](input-computer-science.md). If any coordinate is unread, two completions differing only at that coordinate follow the same observed [graph path](path-in-a-graph.md) but have opposite [parity](parity.md). A single leaf cannot correctly label both.

The same argument works for $n$ [bits](bit.md): [parity](parity.md) needs all $n$ queries on every [input](input-computer-science.md), whatever their order. Thus its [decision-tree depth](decision-tree-depth.md) is $n$, its [expected query cost](expected-query-cost.md) is $n$ for every [input](input-computer-science.md) [probability distribution](probability-distribution-split.md), and each [coordinate revealment](coordinate-revealment.md) is one. The algorithm remains required to be correct on the whole [Boolean cube](boolean-hypercube.md), even if the chosen [probability distribution](probability-distribution-split.md) assigns some [inputs](input-computer-science.md) zero [probability](probability.md); a promise restricting permitted [inputs](input-computer-science.md) would be a different [computational problem](computational-problem.md).

## ↑ Ancestors (6)

1. [Decision tree](decision-tree.md)
2. [Decision tree model](decision-tree-model.md)
3. [Computational complexity theory](computational-complexity-theory.md)
4. [Theoretical computer science](theoretical-computer-science-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Three-bit majority decision tree](three-bit-majority-decision-tree.md)
