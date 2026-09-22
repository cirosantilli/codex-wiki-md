# Decision-tree depth

↑ **Parent:** [Decision tree](decision-tree.md)

The [decision-tree depth](decision-tree-depth.md) $D(f)$ of a [Boolean function](boolean-function.md) $f$ is the smallest possible maximum number of [input](input-computer-science.md) coordinates queried along any root-to-leaf [graph path](path-in-a-graph.md) of a [decision tree](decision-tree.md) computing $f$:

$$
D(f)=\min_{T\text{ computes }f}\max_{x\in\{0,1\}^n}q_T(x)=\min_{T\text{ computes }f}h(T).
$$

The actual depth $h(T)$ of a particular [decision tree](decision-tree.md) can exceed this optimum. A [constant function](constant-function.md) admits a depth-zero tree even though an inefficient algorithm could inspect its entire [input](input-computer-science.md) before returning that constant. [Expected query cost](expected-query-cost.md) and [coordinate revealment](coordinate-revealment.md) additionally require an [input](input-computer-science.md) [probability distribution](probability-distribution-split.md); $D(f)$ does not. The [three-bit majority decision tree](three-bit-majority-decision-tree.md) and three-[bit](bit.md) [parity](parity.md) both have optimal [decision-tree depth](decision-tree-depth.md) three, although only the former has the two-query shortcuts described above.

**Table of contents**

- [Certificate complexity of a Boolean function](certificate-complexity-of-a-boolean-function.md)
  - [Query certificate](query-certificate.md)
- [Evasive Boolean function](evasive-boolean-function.md)
  - [Alternating-sum criterion for decision-tree evasiveness](alternating-sum-criterion-for-decision-tree-evasiveness.md)
- [Decision-tree adversary for a threshold function](decision-tree-adversary-for-a-threshold-function.md)

## ↑ Ancestors (6)

1. [Decision tree](decision-tree.md)
2. [Decision tree model](decision-tree-model.md)
3. [Computational complexity theory](computational-complexity-theory.md)
4. [Theoretical computer science](theoretical-computer-science-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Common-center graph property](common-center-graph-property.md)
- [Decision-tree depth](decision-tree-depth.md)
- [Decision-tree query cost](decision-tree-query-cost.md)
- [Parity lower bound for Boolean queries](parity-lower-bound-for-boolean-queries.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-59/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-124/1/iii/solution.md)
- [Three-bit majority decision tree](three-bit-majority-decision-tree.md)
