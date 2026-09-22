<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [well-quasi-ordering](../../../../../well-quasi-ordering.md) is a [preorder](../../../../../preorder.md) $(Q,\le)$ such that every infinite [sequence](../../../../../sequence.md) $(x_n)$ has indices $i<j$ with $x_i\le x_j$. Reflexivity and transitivity are part of the definition; antisymmetry is unnecessary. An infinite [sequence](../../../../../sequence.md) without such a pair is a [bad sequence](../../../../../bad-sequence.md).

The [perfect subsequence lemma](../../../../../perfect-subsequence-lemma.md) strengthens this definition: **every infinite [sequence](../../../../../sequence.md) in a [well-quasi-order](../../../../../well-quasi-ordering.md) has an infinite nondecreasing [subsequence](../../../../../subsequence.md)**, meaning

$$
\boxed{i_0<i_1<\cdots,\qquad x_{i_r}\le x_{i_s}\quad(r<s).}
$$

Here is a proof that does not assume the lemma implicitly. There must be an index $i$ with infinitely many later indices $j$ satisfying $x_i\le x_j$. Otherwise each index would have only finitely many such successors. Starting with any index, choose the next one beyond the [union](../../../../../set-union.md) of those finite successor [sets](../../../../../set-split.md) for the previously chosen indices. This constructs a [bad sequence](../../../../../bad-sequence.md), contradicting the [well-quasi-ordering](../../../../../well-quasi-ordering.md) property.

Choose $i_0$ with infinitely many successors above it, and restrict to those successors. Apply the same argument to that infinite [subsequence](../../../../../subsequence.md), obtaining $i_1>i_0$ with infinitely many later successors above it within the restricted [sequence](../../../../../sequence.md). Continue. Every subsequent restriction lies inside all previous upper cones, so $x_{i_r}\le x_{i_s}$ for every $r<s$. This proves the lemma, including for a genuine [quasi-order](../../../../../preorder.md) with distinct equivalent elements. Both alternatives below use it.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
