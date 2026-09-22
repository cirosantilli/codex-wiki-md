# Decision tree

↑ **Parent:** [Decision tree model](decision-tree-model.md)

A [decision tree](decision-tree.md) represents a [deterministic computation](deterministic-computation.md) of a known [Boolean function](boolean-function.md) $f:\{0,1\}^n\to\{0,1\}$ by inspecting [input](input-computer-science.md) [bits](bit.md). Each internal [vertex](vertex-graph-theory.md) of its [binary tree](binary-tree.md) names a coordinate $i$ to query, its two outgoing [edges](edge-of-a-graph.md) carry answers 0 and 1, and each leaf carries the [output](output-computing.md) 0 or 1. Starting at the [root of a tree](root-of-a-tree.md), read the named [bit](bit.md), follow its answer [edge](edge-of-a-graph.md), and repeat until a leaf is reached. Correctness requires the leaf's label to equal $f(x)$ for every [input](input-computer-science.md) $x$.[Buhrman and de Wolf, Complexity Measures and Decision Tree Complexity: A Survey, section 3.1, manuscript p. 5: deterministic trees and D(f)](complexity-measures-and-decision-tree-complexity-a-survey-by-harry-buhrman-and-ronald-de-wolf.md)

The next coordinate, or the decision to stop, can depend on earlier answers: this is adaptive querying. The same [input](input-computer-science.md) always follows the same [graph path](path-in-a-graph.md); adaptivity does not require randomness. A correct leaf must have the same [output](output-computing.md) for every completion of the observed [bits](bit.md). Thus a [decision tree](decision-tree.md) can stop as soon as the observations form a [query certificate](query-certificate.md). Querying an already known coordinate adds no information, so we use [decision trees](decision-tree.md) without repeated coordinates on a [graph path](path-in-a-graph.md); an efficient tree also removes queries made after the [output](output-computing.md) is already forced.

The motivation is exact computation with shortcuts. If inspecting an [input](input-computer-science.md) entry is expensive, the question is how much of the [input](input-computer-science.md) must actually be read. The [decision-tree query cost](decision-tree-query-cost.md) counts these inspections, while local calculations on known values are free in this model; this cost need not equal an implementation's [time complexity](time-complexity.md). Here the [Boolean function](boolean-function.md) is specified in advance and must be computed exactly on every [input](input-computer-science.md). [Decision tree learning](decision-tree-learning.md) instead fits a predictor from data, with a different objective.

**Table of contents**

- [Binary decision tree](binary-decision-tree.md)
- [Three-bit majority decision tree](three-bit-majority-decision-tree.md)
- [Parity lower bound for Boolean queries](parity-lower-bound-for-boolean-queries.md)
- [Decision-tree query cost](decision-tree-query-cost.md)
  - [Expected query cost](expected-query-cost.md)
  - [Coordinate revealment](coordinate-revealment.md)
- [Decision-tree depth](decision-tree-depth.md)
  - [Certificate complexity of a Boolean function](certificate-complexity-of-a-boolean-function.md)
    - [Query certificate](query-certificate.md)
  - [Evasive Boolean function](evasive-boolean-function.md)
    - [Alternating-sum criterion for decision-tree evasiveness](alternating-sum-criterion-for-decision-tree-evasiveness.md)
  - [Decision-tree adversary for a threshold function](decision-tree-adversary-for-a-threshold-function.md)

## ↑ Ancestors (5)

1. [Decision tree model](decision-tree-model.md)
2. [Computational complexity theory](computational-complexity-theory.md)
3. [Theoretical computer science](theoretical-computer-science-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (23)

- [Binary search](binary-search.md)
- [Circuit size](circuit-size.md)
- [Comparison sorting lower bound](comparison-sorting-lower-bound.md)
- [Coordinate revealment](coordinate-revealment.md)
- [Decision stump](decision-stump.md)
- [Decision tree](decision-tree.md)
- [Decision-tree depth](decision-tree-depth.md)
- [Decision-tree query cost](decision-tree-query-cost.md)
- [Disjunctive normal form](disjunctive-normal-form.md)
- [Evasive Boolean function](evasive-boolean-function.md)
- [Expected query cost](expected-query-cost.md)
- [Håstad switching lemma](hastad-switching-lemma.md)
- [OSSS inequality](osss-inequality.md)
- [Parity lower bound for Boolean queries](parity-lower-bound-for-boolean-queries.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-39/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/4h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/4h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/4g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-59/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-59/4/c/solution.md)
- [Three-bit majority decision tree](three-bit-majority-decision-tree.md)
