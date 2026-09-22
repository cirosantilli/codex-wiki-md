<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose a [tree parent](../../../../../parent-in-a-rooted-tree.md) at depth $n-1$, with $n<L$, has an unused outgoing digit. The missing [tree child](../../../../../child-in-a-rooted-tree.md) gives an empty [code tree](../../../../../prefix-tree-of-a-code.md) branch at depth $n$. Move any deepest [tree leaf](../../../../../leaf-of-a-tree.md) into that position, retaining all other [codewords](../../../../../codeword.md) and deleting the abandoned empty branch. The new word has no old word as a prefix, because it lies in an unused branch, and it is not a prefix of any retained word. Its length decreases from $L$ to $n$. With a [full-support finite distribution](../../../../../full-support-probability-distribution-on-a-finite-alphabet.md) this reduces [expected codeword length](../../../../../expected-codeword-length.md) by $p_i(L-n)>0$, contradicting optimality. Hence all three [tree children](../../../../../child-in-a-rooted-tree.md) exist, and each has a descendant [codeword](../../../../../codeword.md). In fact **every internal [vertex](../../../../../vertex-graph-theory.md) above depth $L-1$ has all three [tree children](../../../../../child-in-a-rooted-tree.md)**. Applying this to the [tree parent](../../../../../parent-in-a-rooted-tree.md) of the specified prefix gives the claimed three extensions.

The positive-probability qualification attached only to the specified prefix does not by itself suffice. In the zero-weight example $(p,c)=((1,0,0),(0,10,110))$, choose the positive-probability word $0$, so $n=1<L=3$. There is no word starting with $2$. The deepest [tree leaf](../../../../../leaf-of-a-tree.md) available for relocation has [probability](../../../../../probability.md) zero, so the strict-improvement argument fails. This is why the [full-support finite distribution](../../../../../full-support-probability-distribution-on-a-finite-alphabet.md) assumption is used for the structural conclusions.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
