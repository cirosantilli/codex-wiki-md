# Nonunique optimal prefix code

↑ **Parent:** [Optimal prefix code](optimal-prefix-code.md)

An [optimal prefix code](optimal-prefix-code.md) can be nonunique in several different senses. Exchanging the $0,1$ labels on the outgoing [edges](edge-of-a-graph.md) of an internal [vertex](vertex-graph-theory.md) changes [codewords](codeword.md) while preserving every symbol's [codeword length](codeword-length.md), the [code tree](prefix-tree-of-a-code.md) shape, and [expected codeword length](expected-codeword-length.md). This freedom exists even with strictly unequal [probabilities](probability.md). Exchanging equal-probability symbols between leaves also preserves [expected codeword length](expected-codeword-length.md); if their [leaf depths in a code tree](leaf-depth-in-a-code-tree.md) differ, their individual [codeword lengths](codeword-length.md) change, though the set of leaf depths does not. For example, three equiprobable symbols have optimal [codeword lengths](codeword-length.md) $(1,2,2)$: any of the three can receive the one-[bit](bit.md) [codeword](codeword.md).[p. 1099, Derived Coding Requirements: equal-probability messages may have unequal lengths and may exchange codes without changing the mean](a-method-for-the-construction-of-minimum-redundancy-codes-by-david-a-huffman.md)

Ties between weights of entire [subtrees](subtree.md) during [Huffman coding](huffman-coding.md) can go further and change the [code tree](prefix-tree-of-a-code.md) shape and its collection of [codeword lengths](codeword-length.md). Take $(p_A,p_B,p_C,p_D)=(0.4,0.2,0.2,0.2)$ and first merge $C,D$, creating weight $0.4$. Next, $B$ of weight $0.2$ can merge either with $A$ or with the $CD$ [subtree](subtree.md), both of weight $0.4$. The two resulting [prefix codes](prefix-code.md) are

$$
\begin{array}{c|cccc|c}
&c(A)&c(B)&c(C)&c(D)&L(c)\\\hline
\text{balanced}&00&01&10&11&2\\
\text{unequal depths}&0&10&110&111&2
\end{array}
$$

For the second [prefix code](prefix-code.md), $L=0.4\cdot1+0.2\cdot2+0.2\cdot3+0.2\cdot3=2$ [bits](bit.md). Both merge sequences add weights $0.4,0.6,1$, whose sum is $2$. Enumerating the [full binary trees](full-binary-tree.md) with four leaves also proves optimality independently: $(2,2,2,2)$ costs $2$, while the least cost of $(1,2,3,3)$ is again $2$. The two [code trees](prefix-tree-of-a-code.md) cannot be obtained from each other merely by relabelling leaves or exchanging [edge](edge-of-a-graph.md) labels: their collections of [leaf depths in a code tree](leaf-depth-in-a-code-tree.md) differ.

<a id="tied-huffman-weights-distinct-optimal-trees"></a>
![](tied-huffman-weights-distinct-optimal-trees.png)

**[Figure 24](#tied-huffman-weights-distinct-optimal-trees). A tie between a symbol and a merged subtree gives two optimal prefix trees, with depths 2,2,2,2 and 1,2,3,3**.

The quantifier in the [Huffman sibling property](huffman-sibling-property.md) is visible here too. Choose $B,C$ as two least-probability symbols. In the displayed balanced [optimal prefix code](optimal-prefix-code.md), they are not [sibling leaves in a code tree](sibling-leaves-in-a-code-tree.md). Exchanging $B,D$, which have equal [probabilities](probability.md), produces another balanced [optimal prefix code](optimal-prefix-code.md) in which $B,C$ are deepest [sibling leaves in a code tree](sibling-leaves-in-a-code-tree.md). Thus the proof supplies an optimal representative with the chosen pair together. It does not force that labelling on every optimum. An implementation can make its tie choices and $0/1$ [edge](edge-of-a-graph.md) assignments deterministic when encoder and decoder need to reproduce the same [codewords](codeword.md); optimal mean length alone does not specify them.

## ↑ Ancestors (7)

1. [Optimal prefix code](optimal-prefix-code.md)
2. [Huffman coding](huffman-coding.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/3i/b/solution.md)
