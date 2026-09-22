# Shape of minimum-cost positive-weight ternary prefix trees

↑ **Parent:** [Ternary prefix code](ternary-prefix-code.md)

For a finite source [alphabet](alphabet.md) with at least two symbols and strictly positive weights, every [ternary prefix code](ternary-prefix-code.md) minimizing weighted [codeword length](codeword-length.md) has all internal [vertices](vertex-graph-theory.md) of [outdegree](outdegree.md) three, except possibly one of [outdegree](outdegree.md) two whose [tree children](child-in-a-rooted-tree.md) are deepest [tree leaves](leaf-of-a-tree.md).

To prove this, let $L$ be the greatest [tree leaf](leaf-of-a-tree.md) depth. A missing [tree child](child-in-a-rooted-tree.md) at any depth $n<L$ would permit moving a deepest [tree leaf](leaf-of-a-tree.md) into that vacant branch, strictly reducing its positive weighted cost. Thus all internal [vertices](vertex-graph-theory.md) above depth $L-1$ have three [tree children](child-in-a-rooted-tree.md). [Tree parents](parent-in-a-rooted-tree.md) at depth $L-1$ have only [tree leaves](leaf-of-a-tree.md) as [tree children](child-in-a-rooted-tree.md); one [tree child](child-in-a-rooted-tree.md) would permit contraction and strict improvement. If two such [tree parents](parent-in-a-rooted-tree.md) each had two [tree children](child-in-a-rooted-tree.md), move one [tree child](child-in-a-rooted-tree.md) of the second into the first [tree parent](parent-in-a-rooted-tree.md)'s third slot, preserving its depth, and contract the second [tree parent](parent-in-a-rooted-tree.md)'s remaining [tree child](child-in-a-rooted-tree.md). This again strictly improves cost. There is therefore at most one binary [tree parent](parent-in-a-rooted-tree.md). If the number of symbols is an [odd number](odd-number.md), the leaf-count formula for a [full ternary tree](full-ternary-tree.md) forces $N_2$ to be an [even integer](even-number.md); since $N_2\leq1$, there is no binary [tree parent](parent-in-a-rooted-tree.md).

Strict positivity matters. For [probabilities](probability.md) $(1,0,0)$, the [prefix code](prefix-code.md) $(0,10,110)$ minimizes [expected codeword length](expected-codeword-length.md) at one [trit](trit.md), yet has unary [vertices](vertex-graph-theory.md) and a deepest [tree leaf](leaf-of-a-tree.md) without a [sibling codeword](sibling-leaves-in-a-code-tree.md). Removing or rearranging zero-weight branches can select a reduced minimizer, but arbitrary minimizers need not have the positive-weight shape.

## ↑ Ancestors (9)

1. [Ternary prefix code](ternary-prefix-code.md)
2. [Prefix code](prefix-code.md)
3. [Decipherable code](decipherable-code.md)
4. [Unique decodability](unique-decodability.md)
5. [Coding theory](coding-theory-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [B](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/2/b.md)
- [Ternary Huffman coding](ternary-huffman-coding.md)
