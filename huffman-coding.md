# Huffman coding

↑ **Parent:** [Information theory](information-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Huffman_coding)

Huffman coding makes frequent symbols cheap to store by giving them short [codewords](codeword.md), while allowing rare symbols longer [codewords](codeword.md). For a known [probability distribution](probability-distribution.md) on a finite [alphabet](alphabet.md) with at least two positive-probability symbols, binary Huffman coding constructs a [prefix code](prefix-code.md) minimizing [expected codeword length](expected-codeword-length.md) among binary [prefix codes](prefix-code.md) that encode one source symbol at a time. The objective is an average under that [probability distribution](probability-distribution.md); it does not promise to shorten every message. Encoder and decoder must agree on the resulting [Huffman code](huffman-code.md). [Symbol Codes by Ben Lynn](symbol-codes-by-ben-lynn.md)

The construction grows a [binary tree](binary-tree.md) from its leaves towards its [root of a tree](root-of-a-tree.md). Start with one leaf per symbol, weighted by its [probability](probability.md). Repeatedly join the two currently smallest weights beneath a new [parent in a rooted tree](parent-in-a-rooted-tree.md), whose weight is their sum, and replace the pair by that [subtree](subtree.md). Include newly formed [subtrees](subtree.md) when choosing the next pair. When one [tree](tree-graph-theory.md) remains, label the two outgoing [edges](edge-of-a-graph.md) at every internal [vertex](vertex-graph-theory.md) with $0$ and $1$; the labels on the [graph path](path-in-a-graph.md) from the [root of a tree](root-of-a-tree.md) to a symbol give its [codeword](codeword.md). This is a [greedy algorithm](greedy-algorithm.md): each step makes a locally cheapest merge, yet the result is an [optimal prefix code](optimal-prefix-code.md).

For a concrete example, use [probabilities](probability.md) $p_A=0.4$, $p_B=0.3$, $p_C=0.2$, $p_D=0.1$. First join $D$ and $C$, creating weight $0.3$. The remaining weights are $0.3$ for $B$, $0.3$ for the $CD$ [subtree](subtree.md), and $0.4$ for $A$. Join the two $0.3$ weights to make $0.6$, then join $A$ with that $0.6$ [subtree](subtree.md) to make $1$. The merge weights are therefore $0.3,0.6,1$. Each merge adds one [bit](bit.md) to every [codeword](codeword.md) below it, so their sum is the [expected codeword length](expected-codeword-length.md): $0.3+0.6+1=1.9$ [bits](bit.md) per source symbol. The diagram fixes the [edge](edge-of-a-graph.md) labels to produce the [Huffman code](huffman-code.md) used below.

<a id="image-huffman-merges-for-probabilities-0-4-0-3-0-2-0-1-and-their-binary-codewords"></a>
![](huffman-merge-tree-example.png)

**[Figure 27](#image-huffman-merges-for-probabilities-0-4-0-3-0-2-0-1-and-their-binary-codewords). Huffman merges for probabilities 0.4, 0.3, 0.2, 0.1 and their binary codewords**.

The useful insight is that choosing short [codewords](codeword.md) is a resource allocation problem: the [prefix code](prefix-code.md) condition constrains the available [codeword lengths](codeword-length.md) through the [Kraft inequality](kraft-mcmillan-inequality.md). Huffman coding solves this one-symbol problem exactly for the supplied [probability distribution](probability-distribution.md). For repeated emissions of a [memoryless classical information source](memoryless-classical-information-source.md), the same [Huffman code](huffman-code.md) can be applied symbol by symbol. More general compression can exploit dependencies or encode groups of symbols; the one-symbol optimality statement does not compare all such methods.

**Table of contents**

- [Huffman code](huffman-code.md)
  - [Uniform-source Huffman length distribution](uniform-source-huffman-length-distribution.md)
- [Huffman sibling property](huffman-sibling-property.md)
  - [Sibling leaves in a code tree](sibling-leaves-in-a-code-tree.md)
  - [Huffman sibling contraction](huffman-sibling-contraction.md)
- [Optimal prefix code](optimal-prefix-code.md)
  - [Leaf depth in a code tree](leaf-depth-in-a-code-tree.md)
  - [Balancing exchange for a uniform optimal prefix code](balancing-exchange-for-a-uniform-optimal-prefix-code.md)
  - [Expected codeword length](expected-codeword-length.md)
  - [Probability monotonicity of optimal prefix-code lengths](probability-monotonicity-of-optimal-prefix-code-lengths.md)
  - [Deepest sibling property of an optimal prefix code](deepest-sibling-property-of-an-optimal-prefix-code.md)
  - [Nonunique optimal prefix code](nonunique-optimal-prefix-code.md)
- [Huffman codeword length bounds](huffman-codeword-length-bounds.md)

## ↑ Ancestors (5)

1. [Information theory](information-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Deflate compression overhead](deflate-compression-overhead.md)
- [Entropy rate and coding length](entropy-rate-and-coding-length.md)
- [Huffman code](huffman-code.md)
- [Huffman sibling contraction](huffman-sibling-contraction.md)
- [Huffman sibling property](huffman-sibling-property.md)
- [Nonunique optimal prefix code](nonunique-optimal-prefix-code.md)
- [Optimal prefix code](optimal-prefix-code.md)
- [Optimal source code](optimal-source-code.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1/4j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/4g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/4h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/4h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/3i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/3i/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/11k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/3i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1/3k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/3h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/3h/b/solution.md)
