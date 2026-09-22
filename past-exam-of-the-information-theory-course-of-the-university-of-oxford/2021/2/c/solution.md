<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [odd integer](../../../../odd-integer.md) $m\geq3$, [ternary Huffman coding](../../../../ternary-huffman-coding.md) repeatedly merges **three** smallest weights.

Start with one [tree leaf](../../../../leaf-of-a-tree.md) for each source symbol, weighted by its [probability](../../../../probability.md). While more than one weighted object remains, choose the three objects with least weights, create their common [tree parent](../../../../parent-in-a-rooted-tree.md) with weight equal to their sum, and replace the three by that [tree parent](../../../../parent-in-a-rooted-tree.md). Newly created [tree parents](../../../../parent-in-a-rooted-tree.md) participate in subsequent choices. Each merge reduces the number of objects by two; an [odd number](../../../../odd-number.md) of objects therefore reaches three and then one, never an unmergeable pair. The final object is the [tree root](../../../../root-of-a-tree.md) of the [code tree](../../../../prefix-tree-of-a-code.md).

Label the three outgoing [edges](../../../../edge-of-a-graph.md) at each internal [vertex](../../../../vertex-graph-theory.md) by $0,1,2$ in any order. The digits along the root-to-leaf [graph path](../../../../path-in-a-graph.md) give each symbol's [codeword](../../../../codeword.md). [Tree leaves](../../../../leaf-of-a-tree.md) cannot be ancestors of other [tree leaves](../../../../leaf-of-a-tree.md), so this is a [prefix code](../../../../prefix-code.md). Ties can be resolved arbitrarily. The [expected codeword length](../../../../expected-codeword-length.md) is measured in [trits](../../../../trit.md), and equals the sum of all merge weights, because each merge adds one digit to every [codeword](../../../../codeword.md) below it.

The structural reason for merging three is that the positive-weight, odd-leaf case has a [full ternary tree](../../../../full-ternary-tree.md). Its deepest [sibling codeword](../../../../sibling-leaves-in-a-code-tree.md) triple can receive the three least weights by exchanging [tree leaf](../../../../leaf-of-a-tree.md) labels, and contracting that triple reduces the problem by two symbols. This explains the recursive construction; a separate optimality proof is not required here.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
