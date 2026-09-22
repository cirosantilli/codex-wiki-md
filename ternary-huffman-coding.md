# Ternary Huffman coding

↑ **Parent:** [Huffman coding](huffman-coding.md)

The three-symbol output version of [Huffman coding](huffman-coding.md). For an [odd number](odd-number.md) $m\geq3$ of source symbols, repeatedly merge the three least current weights, replacing them by their sum. Each merge reduces the number of weighted objects by two until one [tree root](root-of-a-tree.md) remains. Label each [tree parent](parent-in-a-rooted-tree.md)'s outgoing [edges](edge-of-a-graph.md) $0,1,2$ to obtain a [ternary prefix code](ternary-prefix-code.md). The merge weights sum to the [expected codeword length](expected-codeword-length.md) in [trits](trit.md).

For an [even number](even-number.md) of source symbols, first merge the two least weights, then continue with triples. Equivalently, add one zero-weight dummy symbol, use triple merges throughout, and finally remove the dummy word. Ties may be resolved arbitrarily. This minimizes [expected codeword length](expected-codeword-length.md). The [shape of minimum-cost positive-weight ternary prefix trees](shape-of-minimum-cost-positive-weight-ternary-prefix-trees.md), followed by exchanging the least weights into a deepest [sibling codeword](sibling-leaves-in-a-code-tree.md) triple, reduces the case of an [odd number](odd-number.md) of symbols to the same optimization with two fewer symbols. If there is a binary deepest [tree parent](parent-in-a-rooted-tree.md) when the number of symbols is an [even number](even-number.md), the two least weights can be placed there first. Contracting the chosen [sibling codewords](sibling-leaves-in-a-code-tree.md) changes every competing cost by their fixed weight sum. This gives the same optimal-substructure proof as [Huffman sibling contraction](huffman-sibling-contraction.md), with a triple or the initial pair replacing a binary pair.

## ↑ Ancestors (6)

1. [Huffman coding](huffman-coding.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Full ternary tree](full-ternary-tree.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/2/a/solution.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/2/c/solution.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/2/d/solution.md)
