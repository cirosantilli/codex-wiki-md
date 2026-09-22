# Optimal prefix code

↑ **Parent:** [Huffman coding](huffman-coding.md)

An optimal prefix code minimizes [expected codeword length](expected-codeword-length.md) for a fixed source [probability distribution](probability-distribution-split.md). Here the source [alphabet](alphabet.md) is finite, has $n\geq2$ symbols, and has $p_x>0$ for every symbol; each source symbol receives one [codeword](codeword.md) over the binary output [alphabet](alphabet.md) $\{0,1\}$. Its [code tree](prefix-tree-of-a-code.md) puts the symbols at leaves. Reading the [edges](edge-of-a-graph.md) along the [graph path](path-in-a-graph.md) from the [root of a tree](root-of-a-tree.md) to a leaf produces its [codeword](codeword.md), so the [leaf depth in a code tree](leaf-depth-in-a-code-tree.md) $d_x$ is exactly its [codeword length](codeword-length.md). Thus

$$
L(c)=\sum_xp_xd_x,\qquad
L^*(p)=\min_{c\text{ a binary prefix code}}L(c).
$$

For unnormalized positive weights, minimize $C(T)=\sum_xw_xd_x$ instead; the corresponding [expected codeword length](expected-codeword-length.md) is $C(T)/\sum_xw_x$. This connects the abstract optimization to storage or transmission: $d_x$ counts the [bits](bit.md) charged when symbol $x$ occurs. [Huffman coding](huffman-coding.md) attains this minimum; the [Huffman sibling property](huffman-sibling-property.md) and [Huffman sibling contraction](huffman-sibling-contraction.md) explain why. [Symbol Codes by Ben Lynn](symbol-codes-by-ben-lynn.md)

For $(p_A,p_B,p_C,p_D)=(0.4,0.3,0.2,0.1)$, a balanced [code tree](prefix-tree-of-a-code.md) charges every symbol two [bits](bit.md), giving $L=2$. The [codeword lengths](codeword-length.md) $(1,2,3,3)$ charge the most frequent symbol only one [bit](bit.md), giving $L=1.9$. The choice concerns weighted cost, not just the greatest [codeword length](codeword-length.md): increasing that maximum from two to three can improve the average.

The search over [prefix codes](prefix-code.md) looks infinite, but positivity reduces it to finitely many [full binary trees](full-binary-tree.md) with $n$ leaves. A [vertex](vertex-graph-theory.md) with one child can be suppressed to improve cost, and a [full binary tree](full-binary-tree.md) with $n$ leaves has $n-1$ internal [vertices](vertex-graph-theory.md). There are consequently finitely many such shapes and symbol assignments, so the minimum exists. For four leaves, the only possible sorted [codeword lengths](codeword-length.md) in a [full binary tree](full-binary-tree.md) are $(2,2,2,2)$ and $(1,2,3,3)$. [Probability monotonicity of optimal prefix-code lengths](probability-monotonicity-of-optimal-prefix-code-lengths.md) assigns larger [probabilities](probability.md) to shallower leaves, giving respective minimum costs $2$ and $1.9$ in this example. This is an independent small-instance check of the [Huffman code](huffman-code.md).

These hypotheses matter. With zero weights, suppressing a [subtree](subtree.md) carrying only zero weight need not strictly improve cost, so an [optimal prefix code](optimal-prefix-code.md) need not have a [full binary tree](full-binary-tree.md). A one-symbol source raises the convention of whether an empty [codeword](codeword.md) is allowed. Both cases are outside the original statement here. Encoding groups of symbols changes the source [alphabet](alphabet.md) and the optimization problem; the minimum here concerns one source symbol per [codeword](codeword.md).

**Table of contents**

- [Leaf depth in a code tree](leaf-depth-in-a-code-tree.md)
- [Balancing exchange for a uniform optimal prefix code](balancing-exchange-for-a-uniform-optimal-prefix-code.md)
- [Expected codeword length](expected-codeword-length.md)
- [Probability monotonicity of optimal prefix-code lengths](probability-monotonicity-of-optimal-prefix-code-lengths.md)
- [Deepest sibling property of an optimal prefix code](deepest-sibling-property-of-an-optimal-prefix-code.md)
- [Nonunique optimal prefix code](nonunique-optimal-prefix-code.md)

## ↑ Ancestors (6)

1. [Huffman coding](huffman-coding.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Huffman code](huffman-code.md)
- [Huffman coding](huffman-coding.md)
- [Huffman sibling contraction](huffman-sibling-contraction.md)
- [Huffman sibling property](huffman-sibling-property.md)
- [Nonunique optimal prefix code](nonunique-optimal-prefix-code.md)
- [Optimal prefix code](optimal-prefix-code.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/3i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/3i/a/ii/solution.md)
- [Sibling leaves in a code tree](sibling-leaves-in-a-code-tree.md)
