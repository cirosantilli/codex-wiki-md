# Huffman sibling contraction

↑ **Parent:** [Huffman sibling property](huffman-sibling-property.md)

Replace [sibling leaves in a code tree](sibling-leaves-in-a-code-tree.md) labelled $a,b$ by their common [parent in a rooted tree](parent-in-a-rooted-tree.md), now a leaf labelled $m$ of weight $w_m=w_a+w_b$. All other [codewords](codeword.md) stay fixed; each of $a,b$ loses one [bit](bit.md). For any such [code tree](prefix-tree-of-a-code.md) $T$ and the contracted [code tree](prefix-tree-of-a-code.md) $T'$, their weighted costs satisfy

$$
C(T)=C(T')+w_a+w_b.
$$

If $a,b$ have two least weights, the [Huffman sibling property](huffman-sibling-property.md) gives an [optimal prefix code](optimal-prefix-code.md) containing this pair. Its contracted [prefix code](prefix-code.md) must be optimal for the reduced weights $w'$: any cheaper reduced [prefix code](prefix-code.md) could be expanded at $m$ by appending $0,1$, giving a cheaper original [prefix code](prefix-code.md). Conversely, expanding any optimal reduced [prefix code](prefix-code.md) adds precisely $w_a+w_b$ and attains the original minimum. This is [optimal substructure](optimal-substructure.md), the justification for repeating the merge in [Huffman coding](huffman-coding.md). [Symbol Codes by Ben Lynn](symbol-codes-by-ben-lynn.md)

In the exchange diagram, $C,D$ contract to weight $0.3$ at [leaf depth in a code tree](leaf-depth-in-a-code-tree.md) $2$. The reduced [expected codeword length](expected-codeword-length.md) is $0.4\cdot1+0.3\cdot2+0.3\cdot2=1.6$ [bits](bit.md); expanding restores $1.6+0.3=1.9$ [bits](bit.md). For $n=2$, the reduction leaves one symbol: allow its temporary [codeword](codeword.md) to be empty, of cost zero, so expansion gives the two one-[bit](bit.md) [codewords](codeword.md). This convention is only the terminal reduced problem; the original source has at least two symbols.

## ↑ Ancestors (7)

1. [Huffman sibling property](huffman-sibling-property.md)
2. [Huffman coding](huffman-coding.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Optimal prefix code](optimal-prefix-code.md)
