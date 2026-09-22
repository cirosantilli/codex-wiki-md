<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [clique decision problem](../../../../../clique-decision-problem.md) is a [decidable language](../../../../../recursive-language.md): on a valid finite [graph](../../../../../graph-split.md) and an [integer](../../../../../integer-split.md) $k$, reject if $k$ exceeds the number of [vertices](../../../../../vertex-graph-theory.md), and otherwise examine all $k$-element [subsets](../../../../../subset.md) of [vertices](../../../../../vertex-graph-theory.md), accepting if one is a [clique](../../../../../clique-graph-theory.md). Each candidate can be checked by examining all its pairs of distinct [vertices](../../../../../vertex-graph-theory.md). This finite search gives at least one [Turing machine](../../../../../turing-machine.md) deciding the problem, without any claim of [polynomial time](../../../../../polynomial-time.md).

By [well-ordering](../../../../../well-order.md) of the [natural numbers](../../../../../natural-number.md), there is a least state count $n_0$ among [Turing machines](../../../../../turing-machine.md) deciding the [clique decision problem](../../../../../clique-decision-problem.md). For every $n\geq n_0$, add $n-n_0$ unreachable states to a machine with $n_0$ states. Its behaviour on every [input](../../../../../input-computer-science.md) is unchanged, and it has exactly $n$ states. For $n<n_0$ there is no such machine, by minimality. Thus

$$
\boxed{\mathcal L_{\mathrm{cliqueTM}}
=\{\operatorname{enc}(n):n\geq n_0\}.}
$$

A [Turing machine](../../../../../turing-machine.md) with the fixed constant $n_0$ in its description decides this [threshold language](../../../../../threshold-language.md) by validating the [input](../../../../../input-computer-science.md) and comparing its value with $n_0$. **The argument proves the existence of a decider; it does not compute the smallest possible [clique decision problem](../../../../../clique-decision-problem.md) decider.** There is no need to search through machine descriptions and attempt to certify their behaviour on every [input](../../../../../input-computer-science.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
