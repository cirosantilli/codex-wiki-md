# Word metric

↑ **Parent:** [Cayley graph](cayley-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Word_metric)

The [word metric](word-metric.md) measures how many allowed moves are needed to change one [group element](group-element.md) into another. For a finite symmetric [generating set of a group](generating-set-of-a-group.md) $S$ with $1\notin S$, it is the [graph distance](distance-graph-theory.md) between [vertices](vertex-graph-theory.md) of the [Cayley graph](cayley-graph.md), equivalently

$$
d_S(g,h)=|g^{-1}h|_S.
$$

Here [word length](word-length.md) counts letters in a shortest representative of $g^{-1}h$. The [path metric](path-metric.md) on the entire [Cayley graph](cayley-graph.md) also permits points inside [edges](edge-of-a-graph.md); the [word metric](word-metric.md) is its restriction to the [group](group-split.md) itself.[Bridson, Section 1.6 and the remark after Example 1.8](https://people.maths.ox.ac.uk/bridson/papers/BATH97.pdf)

The [word metric](word-metric.md) is left invariant:

$$
d_S(ag,ah)=|(ag)^{-1}(ah)|_S=|g^{-1}h|_S=d_S(g,h).
$$

This corresponds to the label-preserving [group action](group-action.md) on the [Cayley graph](cayley-graph.md). Symmetry follows by reversing a shortest [graph path](path-in-a-graph.md); concatenating routes gives the [triangle inequality](triangle-inequality.md).[Mann, Groups, geometry, and rigidity, Definition 1.1](https://webusers.imj-prg.fr/~kathryn.mann/classes/GGRminicourse.pdf)

Right invariance can fail in a [non-abelian group](non-abelian-group.md), because right multiplication replaces $g^{-1}h$ by $a^{-1}g^{-1}ha$ through [conjugation](conjugation.md). In the [free group](free-group.md) $F(x,y)$ with $S=\{x,x^{-1},y,y^{-1}\}$, we have $d_S(1,y)=1$, whereas $d_S(x,yx)=|x^{-1}yx|_S=3$: the latter [freely reduced word](freely-reduced-word.md) has three letters. In an [abelian group](abelian-group.md), [conjugation](conjugation.md) fixes each element, so right invariance does hold. [Cayley graphs of the integers](cayley-graphs-of-the-integers.md) and [word metric balls in the integer lattice](word-metric-balls-in-the-integer-lattice.md) give examples where the [word metric](word-metric.md) can be calculated explicitly.

**Table of contents**

- [Word metric ball](word-metric-ball.md)
  - [Word metric balls in the integer lattice](word-metric-balls-in-the-integer-lattice.md)
- [Word length](word-length.md)
- [Stable word length](stable-word-length.md)
- [Equivalence of finite word metrics](equivalence-of-finite-word-metrics.md)

## ↑ Ancestors (6)

1. [Cayley graph](cayley-graph.md)
2. [Geometric group theory](geometric-group-theory-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (25)

- [Cayley graph](cayley-graph.md)
- [Cayley graphs of the integers](cayley-graphs-of-the-integers.md)
- [Equivalence of finite word metrics](equivalence-of-finite-word-metrics.md)
- [Growth function of a finitely generated group](growth-function-of-a-finitely-generated-group.md)
- [Milnor–Švarc lemma](milnor-svarc-lemma.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-16/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-19/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-133/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-133/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-133/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-133/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-143/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-133/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-133/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-133/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-133/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-133/3/c/solution.md)
- [Polynomial growth of properly discontinuous isometry groups](polynomial-growth-of-properly-discontinuous-isometry-groups.md)
- [Stable word length](stable-word-length.md)
- [Word metric](word-metric.md)
- [Word metric ball](word-metric-ball.md)
- [Word metric balls in the integer lattice](word-metric-balls-in-the-integer-lattice.md)
